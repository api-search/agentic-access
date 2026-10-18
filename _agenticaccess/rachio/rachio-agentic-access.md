---
acting_count: 49
action_class_counts:
  acting: 49
  connected: 30
api_specs:
- filename: rachio-public-api-openapi.yml
  format: yaml
  label: Rachio Public API
  slug: rachio-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rachio/refs/heads/main/openapi/rachio-public-api-openapi.yml
- filename: rachio-lightingservice-api-openapi.yml
  format: yaml
  label: Rachio Lighting Service API
  slug: rachio-lightingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rachio/refs/heads/main/openapi/rachio-lightingservice-api-openapi.yml
- filename: rachio-programservice-api-openapi.yml
  format: yaml
  label: Rachio Program Service API
  slug: rachio-programservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rachio/refs/heads/main/openapi/rachio-programservice-api-openapi.yml
- filename: rachio-propertyservice-api-openapi.yml
  format: yaml
  label: Rachio Property Service API
  slug: rachio-propertyservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rachio/refs/heads/main/openapi/rachio-propertyservice-api-openapi.yml
- filename: rachio-public-api-openapi.yml
  format: yaml
  label: Rachio Public API
  slug: rachio-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rachio/refs/heads/main/openapi/rachio-public-api-openapi.yml
- filename: rachio-summaryservice-api-openapi.yml
  format: yaml
  label: Rachio Summary Service API
  slug: rachio-summaryservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rachio/refs/heads/main/openapi/rachio-summaryservice-api-openapi.yml
- filename: rachio-valveservice-api-openapi.yml
  format: yaml
  label: Rachio Valve Service API
  slug: rachio-valveservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rachio/refs/heads/main/openapi/rachio-valveservice-api-openapi.yml
- filename: rachio-webhookservice-api-openapi.yml
  format: yaml
  label: Rachio Webhook Service API
  slug: rachio-webhookservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rachio/refs/heads/main/openapi/rachio-webhookservice-api-openapi.yml
consequence_counts:
  read: 30
  safety-critical: 11
  write: 38
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 11
kind: agentic-access
layout: agentic-access
method: generated
name: Rachio Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /lighting/updateLightingController
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /program/createPlannedRunSkipOverrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /program/createSkipOverrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /program/deletePlannedRunSkipOverrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /program/deleteSkipOverrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /public/device/stop_water
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /public/zone/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /summary/getValveDayViews
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /valve/setDefaultRuntime
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /valve/startWatering
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /valve/stopWatering
operation_count: 79
overview: 'Rachio exposes 79 API operations that an AI agent could call, of which 49 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 38 write, and 11 safety-critical.


  11 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Rachio
provider_slug: rachio
slug: rachio-agentic-access
source_filename: rachio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/rachio-api-settings-openapi.yml, openapi/rachio-property-service-openapi.yml,\n  openapi/rachio-smart-hose-timer-openapi.yml, openapi/rachio-smart-lighting-controller-openapi.yml,\n  openapi/rachio-webhooks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 79\n  by_action_class:\n    connected: 30\n    acting: 49\n  by_consequence:\n    read: 30\n    write: 38\n    safety-critical: 11\n  human_in_the_loop_required: 11\noperations:\n- path: /public/device/:id\n  method: get\n  operationId: publicdeviceid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/device/off\n\
  \  method: put\n  operationId: publicdeviceoff-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/device/on\n  method: put\n  operationId: publicdeviceon-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/device/pause_zone_run\n  method: put\n  operationId: publicdevicepause_zone_run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /public/device/rain_delay\n  method: put\n  operationId: devicerain_delay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/device/resume_zone_run\n  method: put\n  operationId: publicdeviceresume_zone_run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/device/stop_water\n  method: put\n  operationId: devicestop_water\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/notification/:deviceId/webhook\n  method: get\n  operationId: publicnotificationdeviceidwebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/notification/webhook\n  method: put\n  operationId: publicnotificationwebhook-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/notification/webhook\n  method: post\n  operationId: publicnotificationwebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/notification/webhook_event_type\n  method: get\n  operationId: publicnotificationwebhook_event_type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/person/info\n  method: get\n  operationId: publicpersoninfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/schedulerule/seasonal_adjustment\n  method: put\n  operationId: publicscheduleruleseasonal_adjustment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/schedulerule/skip\n  method: put\n  operationId: scheduleruleskip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/schedulerule/skip_forward_zone_run\n  method: put\n  operationId: publicscheduleruleskip_forward_zone_run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/schedulerule/start\n  method: put\n  operationId: schedulerulestart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/zone/disable\n  method: put\n  operationId: publiczonedisable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/zone/enable\n  method: put\n  operationId: publiczoneenable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/zone/setMoistureLevel\n  method: put\n  operationId:\
  \ publiczonesetmoisturelevel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/zone/setMoisturePercent\n  method: put\n  operationId: publiczonesetmoisturepercent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/zone/start\n  method: put\n  operationId: zonestart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /public/zone/start_multiple\n  method: put\n  operationId: publiczonestart_multiple\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /property/findPropertyByEntity\n  method: get\n  operationId: PropertyService_FindPropertyByEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/getProperty/{id}\n  method: get\n  operationId: PropertyService_GetProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/listProperties/{userId}\n  method: get\n  operationId: PropertyService_ListProperties\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /program/createPlannedRunSkipOverrides\n  method: post\n  operationId: ProgramService_CreatePlannedRunSkipOverrides\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /program/createProgramV2\n  method: post\n  operationId: ProgramService_CreateProgramV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /program/createSkipOverrides\n  method: post\n  operationId:\
  \ ProgramService_CreateSkipOverrides\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /program/deletePlannedRunSkipOverrides\n  method: post\n  operationId: ProgramService_DeletePlannedRunSkipOverrides\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /program/deleteProgram/{id}\n  method: delete\n  operationId: ProgramService_DeleteProgram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /program/deleteSkipOverrides\n  method: post\n  operationId: ProgramService_DeleteSkipOverrides\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /program/getProgram/{id}\n  method: get\n  operationId: ProgramService_GetProgram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /program/getProgramV2/{id}\n  method: get\n  operationId: ProgramService_GetProgramV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /program/listPrograms/{entityId}\n  method: get\n  operationId: ProgramService_ListPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /program/listProgramsV2\n  method: get\n  operationId: ProgramService_ListProgramsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /program/updateProgramV2\n  method: put\n  operationId: ProgramService_UpdateProgramV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /summary/getValveDayViews\n  method: post\n  operationId: SummaryService_GetValveDayViews\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /valve/getBaseStation/{id}\n  method: get\n  operationId: ValveService_GetBaseStation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valve/getValve/{id}\n  method: get\n  operationId: ValveService_GetValve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valve/listBaseStations/{userId}\n  method: get\n  operationId: ValveService_ListBaseStations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /valve/listValves/{baseStationId}\n  method: get\n  operationId: ValveService_ListValves\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valve/setDefaultRuntime\n  method: put\n  operationId: ValveService_SetDefaultRuntime\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /valve/startWatering\n  method: put\n  operationId: ValveService_StartWatering\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /valve/stopWatering\n  method: put\n  operationId: ValveService_StopWatering\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /lighting/activateLightingScene/{id}\n  method: put\n  operationId: LightingService_ActivateLightingScene\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/createLightingProgram\n  method: post\n  operationId: LightingService_CreateLightingProgram\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/createLightingScene\n  method: post\n  operationId: LightingService_CreateLightingScene\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/createLightingZoneGroup\n  method: post\n  operationId: LightingService_CreateLightingZoneGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /lighting/deactivateLightingScene/{id}\n  method: put\n  operationId: LightingService_DeactivateLightingScene\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/deleteLightingProgram/{id}\n  method: delete\n  operationId: LightingService_DeleteLightingProgram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/deleteLightingScene/{id}\n  method: delete\n  operationId: LightingService_DeleteLightingScene\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/deleteLightingZoneGroup/{id}\n  method: delete\n  operationId: LightingService_DeleteLightingZoneGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/getLightingArea/{id}\n  method: get\n  operationId: LightingService_GetLightingArea\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/getLightingController/{id}\n  method: get\n  operationId: LightingService_GetLightingController\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/getLightingProgram/{id}\n  method: get\n  operationId: LightingService_GetLightingProgram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/getLightingScene/{id}\n  method: get\n  operationId: LightingService_GetLightingScene\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/getLightingZone/{id}\n  method: get\n  operationId: LightingService_GetLightingZone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/getLightingZoneGroup/{id}\n  method: get\n  operationId: LightingService_GetLightingZoneGroup\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/listLightingAreas/{user_id}\n  method: get\n  operationId: LightingService_ListLightingAreas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/listLightingControllers/{lighting_area_id}\n  method: get\n  operationId: LightingService_ListLightingControllers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/listLightingPrograms\n  method: get\n  operationId: LightingService_ListLightingPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/listLightingScenes/{lighting_area_id}\n  method: get\n  operationId:\
  \ LightingService_ListLightingScenes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/listLightingZoneGroups/{lighting_area_id}\n  method: get\n  operationId: LightingService_ListLightingZoneGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/listLightingZones\n  method: get\n  operationId: LightingService_ListLightingZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lighting/setLightingZoneDesiredDimmingSettings\n  method: put\n  operationId: LightingService_SetLightingZoneDesiredDimmingSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/setLightingZoneDimmingLevels\n  method: put\n  operationId: LightingService_SetLightingZoneDimmingLevels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/setLightingZoneStates\n  method: put\n  operationId: LightingService_SetLightingZoneStates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/updateLightingController\n  method: put\n  operationId: LightingService_UpdateLightingController\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /lighting/updateLightingProgram\n  method: put\n  operationId: LightingService_UpdateLightingProgram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/updateLightingScene\n  method: put\n  operationId: LightingService_UpdateLightingScene\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/updateLightingZone\n  method: put\n  operationId: LightingService_UpdateLightingZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lighting/updateLightingZoneGroup\n  method: put\n  operationId: LightingService_UpdateLightingZoneGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/createWebhook\n  method: post\n  operationId: WebhookService_CreateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/deleteAllWebhooks\n  method: delete\n  operationId: WebhookService_DeleteAllWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/deleteWebhook/{id}\n  method: delete\n  operationId: WebhookService_DeleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/getWebhook/{id}\n\
  \  method: get\n  operationId: WebhookService_GetWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/listWebhookEventTypes\n  method: get\n  operationId: WebhookService_ListWebhookEventTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/listWebhooks\n  method: get\n  operationId: WebhookService_ListWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/updateWebhook\n  method: put\n  operationId: WebhookService_UpdateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rachio/refs/heads/main/agentic-access/rachio-agentic-access.yml
summary_line: 79 operations · 49 acting · 11 human-in-the-loop
tags:
- Company
- Smart Home
- IoT
- Irrigation
- Home Automation
- Water Management
- Webhook
---
