---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 7
api_specs:
- filename: devialet-audio-settings-api-openapi.yml
  format: yaml
  label: Devialet Audio Settings API
  slug: devialet-audio-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-audio-settings-api-openapi.yml
- filename: devialet-devices-api-openapi.yml
  format: yaml
  label: Devialet Devices API
  slug: devialet-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-devices-api-openapi.yml
- filename: devialet-groups-api-openapi.yml
  format: yaml
  label: Devialet Groups API
  slug: devialet-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-groups-api-openapi.yml
- filename: devialet-playback-api-openapi.yml
  format: yaml
  label: Devialet Playback API
  slug: devialet-playback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-playback-api-openapi.yml
- filename: devialet-sound-control-api-openapi.yml
  format: yaml
  label: Devialet Sound Control API
  slug: devialet-sound-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-sound-control-api-openapi.yml
- filename: devialet-systems-api-openapi.yml
  format: yaml
  label: Devialet Systems API
  slug: devialet-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/openapi/devialet-systems-api-openapi.yml
consequence_counts:
  read: 7
  safety-critical: 6
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Devialet Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /devices/{deviceId}/resetToFactorySettings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /systems/{systemId}/resetToFactorySettings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /systems/{systemId}/settings/audio/equalizer
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /systems/{systemId}/sources/current/soundControl/volume
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /systems/{systemId}/sources/current/soundControl/volumeDown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /systems/{systemId}/sources/current/soundControl/volumeUp
operation_count: 25
overview: 'Devialet exposes 25 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 12 write, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Devialet
provider_slug: devialet
slug: devialet-agentic-access
source_filename: devialet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/devialet-ip-control-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 7\n    acting: 18\n  by_consequence:\n    read: 7\n    write: 12\n    safety-critical: 6\n  human_in_the_loop_required: 6\noperations:\n- path: /devices/{deviceId}\n  method: get\n  operationId: getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{deviceId}/powerOff\n  method: post\n  operationId: powerOffDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceId}/restart\n  method: post\n  operationId: restartDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceId}/resetToFactorySettings\n  method: post\n  operationId: resetDeviceToFactorySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /systems/{systemId}\n  method: get\n  operationId: getSystem\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /systems/{systemId}/sources/current/soundControl/volume\n  method: get\n  operationId: getSystemVolume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /systems/{systemId}/sources/current/soundControl/volume\n  method: post\n  operationId: setSystemVolume\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /systems/{systemId}/sources/current/soundControl/volumeUp\n  method: post\n  operationId: systemVolumeUp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /systems/{systemId}/sources/current/soundControl/volumeDown\n  method: post\n  operationId: systemVolumeDown\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /systems/{systemId}/settings/audio/equalizer\n  method: get\n  operationId: getSystemEqualizer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /systems/{systemId}/settings/audio/equalizer\n  method: post\n  operationId:\
  \ setSystemEqualizer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /systems/{systemId}/settings/audio/nightMode\n  method: get\n  operationId: getSystemNightMode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /systems/{systemId}/settings/audio/nightMode\n  method: post\n  operationId: setSystemNightMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /systems/{systemId}/bluetooth/startAdvertising\n\
  \  method: post\n  operationId: startSystemBluetoothAdvertising\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /systems/{systemId}/powerOff\n  method: post\n  operationId: powerOffSystem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /systems/{systemId}/restart\n  method: post\n  operationId: restartSystem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /systems/{systemId}/resetToFactorySettings\n  method: post\n  operationId: resetSystemToFactorySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /groups/{groupId}/sources\n  method: get\n  operationId: listGroupSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{groupId}/sources/current\n  method: get\n  operationId: getGroupCurrentSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{groupId}/sources/{sourceId}/playback/play\n\
  \  method: post\n  operationId: playGroupSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}/sources/current/playback/pause\n  method: post\n  operationId: pauseGroupPlayback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}/sources/current/playback/mute\n  method: post\n  operationId: muteGroupPlayback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}/sources/current/playback/unmute\n  method: post\n  operationId: unmuteGroupPlayback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}/sources/current/playback/next\n  method: post\n  operationId: nextGroupTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}/sources/current/playback/previous\n  method: post\n  operationId: previousGroupTrack\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devialet/refs/heads/main/agentic-access/devialet-agentic-access.yml
summary_line: 25 operations · 18 acting · 6 human-in-the-loop
tags:
- Audio
- Consumer Electronics
- Smart Speakers
- Home Automation
- Custom Installation
- Device Control
- Local Network API
- IoT
- Hardware
- Music
- France
---
