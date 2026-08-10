---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 13
api_specs:
- filename: afero-authentication-api-openapi.yml
  format: yaml
  label: Afero Cloud Authentication API
  slug: authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-authentication-api-openapi.yml
- filename: afero-users-api-openapi.yml
  format: yaml
  label: Afero Cloud Users API
  slug: users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-users-api-openapi.yml
- filename: afero-devices-api-openapi.yml
  format: yaml
  label: Afero Cloud Devices API
  slug: devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-devices-api-openapi.yml
- filename: afero-ota-api-openapi.yml
  format: yaml
  label: Afero Cloud OTA Firmware API
  slug: ota-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/openapi/afero-ota-api-openapi.yml
consequence_counts:
  read: 13
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Afero Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Afero exposes 25 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Afero
provider_slug: afero
slug: afero-agentic-access
source_filename: afero-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/afero-authentication-api-openapi.yml, openapi/afero-devices-api-openapi.yml,\n  openapi/afero-ota-api-openapi.yml, openapi/afero-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    acting: 12\n    connected: 13\n  by_consequence:\n    write: 12\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/accounts/{accountId}/devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{accountId}/devices/{deviceId}\n  method: get\n  operationId: getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{accountId}/devices/{deviceId}/actions\n  method: post\n  operationId: executeDeviceAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{accountId}/devices/{deviceId}/friendlyName\n  method: put\n  operationId: updateDeviceFriendlyName\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ota/partners/{partnerId}/types\n  method: post\n  operationId: createFirmwareType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ota/partners/{partnerId}/types\n  method: get\n  operationId: listFirmwareTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ota/partners/{partnerId}/types/{type}\n  method: get\n  operationId: getFirmwareType\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ota/partners/{partnerId}/types/{type}\n  method: put\n  operationId: updateFirmwareType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ota/partners/{partnerId}/pool\n  method: post\n  operationId: createPoolFirmwareImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ota/partners/{partnerId}/pool\n  method: get\n  operationId: listPoolFirmwareImages\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ota/partners/{partnerId}/binaries\n  method: post\n  operationId: uploadFirmwareBinary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ota/partners/{partnerId}/binaries/moveToRepository\n  method: post\n  operationId: moveBinaryToRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ota/partners/{partnerId}/pool/types/{type}\n  method: get\n  operationId: listPoolFirmwareImagesByType\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ota/partners/{partnerId}/pool/types/{type}/names/{name}/versions/{version}/exists\n  method: get\n  operationId: poolFirmwareImageExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ota/partners/{partnerId}/pool/types/{type}/versionNumbers/{versionNumber}/associations\n  method: get\n  operationId: listPoolFirmwareImageAssociations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ota/partners/{partnerId}/pool/types/{type}/versionNumbers/{versionNumber}\n  method: put\n  operationId: updatePoolFirmwareImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ota/partners/{partnerId}/deviceTypes/{deviceTypeId}/firmwareImages\n  method: post\n  operationId: createDeviceTypeFirmwareImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ota/partners/{partnerId}/deviceTypes/{deviceTypeId}/firmwareImages\n  method: get\n  operationId: listDeviceTypeFirmwareImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ota/partners/{partnerId}/deviceTypes/{deviceTypeId}/firmwareImages/types/{type}\n  method: get\n  operationId: listDeviceTypeFirmwareImagesByType\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ota/partners/{partnerId}/deviceTypes/{deviceTypeId}/firmwareImages/types/{type}/versionNumbers/{versionNumber}\n  method: get\n  operationId: getDeviceTypeFirmwareImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ota/partners/{partnerId}/deviceTypes/{deviceTypeId}/firmwareImages/types/{type}/versionNumbers/{versionNumber}\n  method: delete\n  operationId: deleteDeviceTypeFirmwareImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ota/partners/{partnerId}/deviceTypes/{deviceTypeId}/firmwareImages/{firmwareImageId}/push\n\
  \  method: put\n  operationId: pushFirmwareImageToDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ota/partners/{partnerId}/tags\n  method: get\n  operationId: listFirmwareTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/me\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afero/refs/heads/main/agentic-access/afero-agentic-access.yml
summary_line: 25 operations · 12 acting
tags:
- Company
- Internet of Things
- IoT Platform
- Connected Devices
- Device Management
- Firmware
- Over-the-Air Updates
- Bluetooth Low Energy
- Embedded Security
- Hardware
---
