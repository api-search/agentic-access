---
acting_count: 417
action_class_counts:
  acting: 417
  connected: 437
api_specs:
- filename: alianza-openapi-original.yml
  format: yaml
  label: Alianza Public API
  slug: alianza-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alianza/refs/heads/main/openapi/alianza-openapi-original.yml
consequence_counts:
  physical: 13
  read: 437
  safety-critical: 14
  write: 390
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 14
kind: agentic-access
layout: agentic-access
method: generated
name: Alianza Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/partition/{partitionId}/account/{accountId}/accountuser/{userId}/resetpassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/partition/{partitionId}/account/{accountId}/accountuser/{userId}/resetpassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/business-line/voicemail-box/{voicemailBoxId}/rpc/reset-pin
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/business-line/voicemail-box/{voicemailBoxId}/rpc/reset-pin
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/device/{macAddress}/metadata/resetencryptionkey
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/device/{macAddress}/metadata/resetencryptionkey
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/partition/{partitionId}/account/{accountId}/emergency-notifications/groups/{type}/{groupId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/partition/{partitionId}/account/{accountId}/emergency-notifications/groups/{type}/{groupId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/emergency-notifications/groups/{type}/{groupId}/execute-test
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/emergency-notifications/groups/{type}/{groupId}/execute-test
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/partition/{partitionId}/account/{accountId}/user/{userId}/resetpassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/partition/{partitionId}/account/{accountId}/user/{userId}/resetpassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/partition/{partitionId}/managementuser/{id}/resetpassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/partition/{partitionId}/managementuser/{id}/resetpassword
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/app-branding/brand-settings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/app-branding/brand-settings/{brandId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/dynamic-inventory/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/dynamic-inventory/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/send-welcome-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/send-welcome-email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/partition/{partitionId}/account/{accountId}/telephonenumber/tn-requests/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/partition/{partitionId}/account/{accountId}/telephonenumber/tn-requests/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/telephonenumber/tn-requests/{orderId}/refresh
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/telephonenumber/tn-requests/{orderId}/refresh
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/partition/{partitionId}/account/{accountId}/user/{userId}/send-welcome-email
operation_count: 854
overview: 'Alianza exposes 854 API operations that an AI agent could call, of which 417 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 437 read, 390 write, 13 physical, and 14 safety-critical.


  14 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Alianza
provider_slug: alianza
slug: alianza-agentic-access
source_filename: alianza-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/alianza-apidocs-swagger2-original.json, openapi/alianza-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 854\n  by_action_class:\n    connected: 437\n    acting: 417\n  by_consequence:\n    read: 437\n    write: 390\n    safety-critical: 14\n    physical: 13\n  human_in_the_loop_required: 14\noperations:\n- path: /v2/address/validate\n  method: get\n  operationId: validateAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/address/typeahead\n  method: get\n  operationId: typeAhead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/address/state/{state}/city/{city}/zipcode\n  method: get\n  operationId: getZipCodeByCityAndState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/authorize/userinfo\n  method: get\n  operationId: getLoginInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/authorize/logout\n  method: put\n  operationId: logOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/authorize/jwt\n  method: post\n  operationId: loginWithJWT\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/authorize\n  method: post\n  operationId: logUserIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/authorize\n  method: put\n  operationId: changePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/authorize/sso\n  method: get\n  operationId: getClientId\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/authorize/sso\n  method: post\n  operationId: getLoginInfo_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/language\n  method: get\n  operationId: getLanguageFromHeader\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/supported-rate-centers\n  method: get\n  operationId: getClosestAvailableRateCenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/job/{jobId}\n  method: get\n\
  \  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/job/input\n  method: post\n  operationId: input\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/job/{jobId}/input\n  method: get\n  operationId: getInput\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/job/{jobId}/output\n  method: get\n  operationId: getOutput\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/job/{jobId}/output-url\n  method: get\n  operationId:\
  \ getOutputUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/deviceinventory/import\n  method: post\n  operationId: importDeviceInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/deviceinventory\n  method: get\n  operationId: allTelephoneNumberCSVReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/deviceinventory\n  method: post\n  operationId: importDeviceInventory_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/deviceinventory/export\n  method: post\n  operationId: getDeviceInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/deviceinventory/delete\n  method: post\n  operationId: deleteDeviceInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/cymbus/partition-group/{partitionId}\n\
  \  method: get\n  operationId: retrieveCymbusPartitionGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cymbus/partition-group\n  method: put\n  operationId: updateCymbusPartitionGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/deviceprovisioning/{macAddress}\n  method: get\n  operationId: getProvisioningByMacAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/deviceprovisioning/account/{accountid}/device/{deviceid}\n  method: get\n  operationId: getProvisioningByMacAddress_1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/inboundrateplanproduct/{ratePlanId}\n  method: get\n  operationId: retrieveInboundRatePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/inboundrateplanproduct\n  method: get\n  operationId: retrieveInboundRatePlanList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/managementuser/{id}\n  method: get\n  operationId: retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/managementuser/{id}\n  method: put\n\
  \  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/managementuser/{id}\n  method: delete\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/managementuser/{id}\n  method: patch\n  operationId: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/managementuser\n  method: get\n  operationId: retrieve_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/managementuser\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/managementuser/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/managementuser/usergroups\n  method: get\n  operationId: getUserGroupCSV\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/managementuser/usergroups\n  method: post\n  operationId: bulkUpdateUserGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/managementuser/validateproperties\n  method: get\n  operationId: validateProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/managementuser/{id}/resetpassword\n  method: put\n  operationId: resetPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/partition/{partitionId}/managementuser/{id}/sso\n  method: get\n  operationId: sso\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}\n  method: get\n  operationId: retrieve_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/is-di-supported\n  method: get\n  operationId: isDISupported\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/setting\n  method:\
  \ get\n  operationId: getAllSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/inboundcarriers\n  method: get\n  operationId: getInboundCarriers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/deviceinventory_2\n  method: get\n  operationId: allTelephoneNumberCSVReport_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/deviceinventory_2\n  method: post\n  operationId: importDeviceInventory_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/data-history\n  method: get\n  operationId: partitionDataHistorySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/localprefixes/export/csv\n  method: get\n  operationId: allTelephoneNumberCSVReport_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/localprefixes/import\n  method: post\n  operationId: importLocalAreas\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/report/portout/csv\n\
  \  method: get\n  operationId: telephoneNumberPortOutCSVReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/portout/csv_2\n  method: get\n  operationId: telephoneNumberPortOutCSVReport2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/emergencynotificationcompliance/csv_2\n  method: get\n  operationId: emergencyNotificationComplianceReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/user\n  method: get\n  operationId: userSummaryReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v2/partition/{partitionId}/report/device\n  method: get\n  operationId: deviceSummaryReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/device/csv\n  method: get\n  operationId: deviceCSVReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/device/csv_2\n  method: get\n  operationId: deviceCSVReport2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/device/csv_3\n  method: get\n  operationId: deviceCSVReport3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v2/partition/{partitionId}/report/tn\n  method: get\n  operationId: telephoneNumberSummaryReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/tn/csv\n  method: get\n  operationId: telephoneNumberCSVReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/tn/csv_2\n  method: get\n  operationId: telephoneNumberCSVReport2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/sip\n  method: get\n  operationId: sipSummaryReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v2/partition/{partitionId}/report/account/csv\n  method: get\n  operationId: accountCSVReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/account/csv_2\n  method: get\n  operationId: accountCSVReport2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/account/csv_3\n  method: get\n  operationId: accountCSVReport3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/accounthistory/enduserchanges\n  method: get\n  operationId: endUserAccountHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/accounthistory/enduserchanges_2\n  method: get\n  operationId: endUserAccountHistory2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/vfax\n  method: get\n  operationId: vFaxSummaryReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/line\n  method: get\n  operationId: mockLineSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/businesslines/csv_2\n  method: get\n  operationId: businessLinesCSVReport2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/deviceregistration/csv_2\n  method: get\n  operationId: deviceRegistrationReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/user-products/csv_2\n  method: get\n  operationId: userProductsReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/specialtylines/csv_2\n  method: get\n  operationId: specialtyLinesReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/contact_center_usage/csv_1\n  method: get\n  operationId: contactCenterUsageReport\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/contact_center_retail/csv_1\n  method: get\n  operationId: contactCenterRetailReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/sip/csv\n  method: get\n  operationId: sipCSVReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/user/csv_2\n  method: get\n  operationId: userCSVReport2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/sip/csv_2\n  method: get\n  operationId: sipCSVReport2\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/user/csv_3\n  method: get\n  operationId: userCSVReport3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/user/csv\n  method: get\n  operationId: userCSVReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/vfax/csv\n  method: get\n  operationId: vFaxCSVReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/vfax/csv_2\n  method: get\n  operationId: vFaxCSVReport2\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/report/msteams/csv_1\n  method: get\n  operationId: msTeamsReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/security/{securityId}\n  method: get\n  operationId: retrieve_4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/security/{securityId}\n  method: put\n  operationId: update_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/security/{securityId}\n\
  \  method: delete\n  operationId: delete_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/security/{securityId}\n  method: patch\n  operationId: patch_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/security\n  method: get\n  operationId: retrieve_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/security\n  method: post\n  operationId:\
  \ create_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/telephonenumber\n  method: get\n  operationId: retrieve_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/telephonenumber\n  method: post\n  operationId: createTelephoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/telephonenumber/{tn}\n  method: get\n  operationId:\
  \ retrieveTelephoneNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/telephonenumber/{tn}\n  method: delete\n  operationId: delete_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/telephonenumber/search\n  method: get\n  operationId: search_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/telephonenumber/{tn}/availability\n  method: get\n  operationId: retrieveTelephoneNumberAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/telephonenumber/bulkimport\n  method: post\n  operationId: bulkInsert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/telephonenumber/bulkimport_2\n  method: post\n  operationId: bulkInsert2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/telephonenumber/exportstatussearch\n  method: get\n  operationId: exportStatusSearch\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/telephonenumber/exportstatussearch_2\n  method: get\n  operationId: exportStatusSearch2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/telephonenumber/{tn}/cooldown/recover\n  method: put\n  operationId: cooldownRecover\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/telephonenumber/{tn}/reserve\n  method: put\n  operationId: reserve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/telephonenumber/{tn}/reserve\n  method: delete\n  operationId: releaseReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/telephonenumber/statussearch\n  method: get\n  operationId: statusSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/telephonenumber/{tn}/fmfmcheck\n  method: get\n  operationId: isTnOffNet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/telephonenumber/export\n  method: get\n  operationId: getInventoryPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/telephonenumber/export_2\n  method: get\n  operationId: getInventoryPlan2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/account/activation/multiple\n  method: post\n  operationId: multipleActivation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/account/activation\n\
  \  method: post\n  operationId: activation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/account\n  method: get\n  operationId: retrieve_6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/account\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/account/search\n  method: get\n  operationId:\
  \ search_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/account/accounthistorysearch\n  method: get\n  operationId: accountHistoryByAccountNumberSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/account/bulkstatuschange\n  method: post\n  operationId: bulkStatusChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/account/bulkstatuschange_2\n  method: post\n  operationId: bulkStatusChange_2\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/partition/{partitionId}/account/frequentlyaccessed\n  method: get\n  operationId: frequentlyAccessed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/account/recentlyaccessed\n  method: get\n  operationId: recentlyAccessed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/partition/{partitionId}/account/validateproperties\n  method: get\n  operationId: validateProperties_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    t\n\n# --- truncated at 32 KB (270 KB total) ---\n# Full\
  \ source: https://raw.githubusercontent.com/api-evangelist/alianza/refs/heads/main/agentic-access/alianza-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alianza/refs/heads/main/agentic-access/alianza-agentic-access.yml
summary_line: 854 operations · 417 acting · 14 human-in-the-loop
tags:
- Company
- Communications
- Cloud Communications
- Voice
- VoIP
- Telecommunications
- UCaaS
- SIP Trunking
- Telephone Numbers
- CPaaS
- Service Providers
---
