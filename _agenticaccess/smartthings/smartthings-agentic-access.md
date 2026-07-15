---
acting_count: 35
action_class_counts:
  acting: 35
  connected: 30
api_specs:
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Devices API
  slug: smartthings-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Device Commands & Status API
  slug: smartthings-device-commands-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Locations API
  slug: smartthings-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Rooms API
  slug: smartthings-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Scenes API
  slug: smartthings-scenes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Rules API
  slug: smartthings-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Capabilities API
  slug: smartthings-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Subscriptions API
  slug: smartthings-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Schedules API
  slug: smartthings-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Apps API
  slug: smartthings-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Installed Apps API
  slug: smartthings-installed-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Presentations API
  slug: smartthings-presentations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings History API
  slug: smartthings-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
- filename: smartthings-openapi.yml
  format: yaml
  label: SmartThings Virtual Devices API
  slug: smartthings-virtual-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/openapi/smartthings-openapi.yml
consequence_counts:
  read: 30
  write: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smartthings Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 65
overview: 'Samsung SmartThings exposes 65 API operations that an AI agent could call, of which 35 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read and 35 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Samsung SmartThings
provider_slug: smartthings
slug: smartthings-agentic-access
source_filename: smartthings-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smartthings-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 65\n  by_action_class:\n    connected: 30\n    acting: 35\n  by_consequence:\n    read: 30\n    write: 35\n  human_in_the_loop_required: 0\noperations:\n- path: /devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices\n  method: post\n  operationId: installDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceId}\n  method: get\n  operationId: getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{deviceId}\n  method: put\n  operationId: updateDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceId}\n  method: delete\n  operationId: deleteDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /devices/{deviceId}/commands\n  method: post\n  operationId: executeDeviceCommands\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceId}/events\n  method: post\n  operationId: createDeviceEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceId}/status\n  method: get\n  operationId: getDeviceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{deviceId}/components/{componentId}/status\n\
  \  method: get\n  operationId: getDeviceComponentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{deviceId}/components/{componentId}/capabilities/{capabilityId}/status\n  method: get\n  operationId: getDeviceCapabilityStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{deviceId}/health\n  method: get\n  operationId: getDeviceHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: post\n  operationId: createLocation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}\n  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{locationId}\n  method: put\n  operationId: updateLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}\n  method: patch\n  operationId: patchLocation\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}\n  method: delete\n  operationId: deleteLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}/rooms\n  method: get\n  operationId: listRooms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{locationId}/rooms\n  method: post\n  operationId: createRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}/rooms/{roomId}\n  method: get\n  operationId: getRoom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{locationId}/rooms/{roomId}\n  method: put\n  operationId: updateRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}/rooms/{roomId}\n  method: delete\n  operationId: deleteRoom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}/modes\n  method: get\n  operationId: listModes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{locationId}/modes\n  method: post\n  operationId: createMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locations/{locationId}/modes/current\n  method: get\n  operationId: getCurrentMode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{locationId}/modes/current\n\
  \  method: put\n  operationId: setCurrentMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scenes\n  method: get\n  operationId: listScenes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scenes\n  method: post\n  operationId: createScene\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scenes/{sceneId}\n  method: get\n  operationId: getScene\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scenes/{sceneId}\n  method: put\n  operationId: updateScene\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scenes/{sceneId}\n  method: delete\n  operationId: deleteScene\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scenes/{sceneId}/execute\n  method: post\n  operationId: executeScene\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rules\n  method: get\n  operationId: listRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rules\n  method: post\n  operationId: createRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rules/{ruleId}\n  method: get\n  operationId: getRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rules/{ruleId}\n  method: put\n  operationId: updateRule\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rules/{ruleId}\n  method: delete\n  operationId: deleteRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rules/{ruleId}/execute\n  method: post\n  operationId: executeRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capabilities\n  method: get\n  operationId: listCapabilities\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capabilities/{capabilityId}/{capabilityVersion}\n  method: get\n  operationId: getCapability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /installedapps\n  method: get\n  operationId: listInstalledApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /installedapps/{installedAppId}\n  method: get\n  operationId: getInstalledApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /installedapps/{installedAppId}\n  method: delete\n  operationId: deleteInstalledApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /installedapps/{installedAppId}/configs\n  method: get\n  operationId: listInstalledAppConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /installedapps/{installedAppId}/events\n  method: post\n  operationId: createInstalledAppEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /installedapps/{installedAppId}/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /installedapps/{installedAppId}/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /installedapps/{installedAppId}/subscriptions\n  method: delete\n  operationId: deleteAllSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /installedapps/{installedAppId}/subscriptions/{subscriptionId}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /installedapps/{installedAppId}/subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /installedapps/{installedAppId}/schedules\n  method: get\n  operationId: listSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /installedapps/{installedAppId}/schedules/{scheduleName}\n  method: post\n  operationId: createSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /installedapps/{installedAppId}/schedules/{scheduleName}\n  method: delete\n  operationId: deleteSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps\n  method: post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{appNameOrId}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{appNameOrId}\n  method: put\n  operationId: updateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{appNameOrId}\n  method: delete\n  operationId: deleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /presentation\n  method:\
  \ get\n  operationId: getPresentation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /presentation/deviceconfig\n  method: get\n  operationId: getDeviceConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /presentation/deviceconfig\n  method: post\n  operationId: createDeviceConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /history/devices\n  method: get\n  operationId: getDeviceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /virtualdevices\n  method: get\n  operationId: listVirtualDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /virtualdevices\n  method: post\n  operationId: createVirtualDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virtualdevices/{deviceId}/events\n  method: post\n  operationId: createVirtualDeviceEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/agentic-access/smartthings-agentic-access.yml
summary_line: 65 operations · 35 acting
tags:
- Smart Home
- IoT
- Home Automation
- Devices
- Samsung
---
