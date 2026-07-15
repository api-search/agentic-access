---
acting_count: 56
action_class_counts:
  acting: 56
  connected: 66
api_specs:
- filename: microsoft-windows-10-winrt-openapi.yml
  format: yaml
  label: Windows Runtime (WinRT) API
  slug: windows-runtime-winrt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-winrt-openapi.yml
- filename: microsoft-windows-10-win32-openapi.yml
  format: yaml
  label: Win32 API
  slug: win32-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-win32-openapi.yml
- filename: microsoft-windows-10-notifications-openapi.yml
  format: yaml
  label: Windows Notifications API
  slug: windows-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-notifications-openapi.yml
- filename: microsoft-windows-10-ml-openapi.yml
  format: yaml
  label: Windows ML API
  slug: windows-ml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-ml-openapi.yml
- filename: microsoft-windows-10-storage-openapi.yml
  format: yaml
  label: Windows Storage API
  slug: windows-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-storage-openapi.yml
- filename: microsoft-windows-10-cortana-openapi.yml
  format: yaml
  label: Windows Cortana API
  slug: windows-cortana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-cortana-openapi.yml
- filename: microsoft-windows-10-ink-openapi.yml
  format: yaml
  label: Windows Ink API
  slug: windows-ink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-ink-openapi.yml
- filename: microsoft-windows-10-composition-openapi.yml
  format: yaml
  label: Windows Composition API
  slug: windows-composition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-composition-openapi.yml
- filename: microsoft-windows-10-directx-openapi.yml
  format: yaml
  label: DirectX Graphics API
  slug: directx-graphics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-directx-openapi.yml
- filename: microsoft-windows-10-media-capture-openapi.yml
  format: yaml
  label: Windows Media Capture API
  slug: windows-media-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-media-capture-openapi.yml
- filename: microsoft-windows-10-networking-openapi.yml
  format: yaml
  label: Windows Networking API
  slug: windows-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-networking-openapi.yml
- filename: microsoft-windows-10-bluetooth-openapi.yml
  format: yaml
  label: Windows Bluetooth API
  slug: windows-bluetooth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-bluetooth-openapi.yml
- filename: microsoft-windows-10-geolocation-openapi.yml
  format: yaml
  label: Windows Geolocation API
  slug: windows-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-geolocation-openapi.yml
- filename: microsoft-windows-10-sensors-openapi.yml
  format: yaml
  label: Windows Sensors API
  slug: windows-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-sensors-openapi.yml
- filename: microsoft-windows-10-hello-openapi.yml
  format: yaml
  label: Windows Hello Authentication API
  slug: windows-hello-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-hello-openapi.yml
- filename: microsoft-windows-10-winui-openapi.yml
  format: yaml
  label: WinUI API
  slug: winui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-winui-openapi.yml
- filename: microsoft-windows-10-background-tasks-openapi.yml
  format: yaml
  label: Windows Background Tasks API
  slug: windows-background-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-background-tasks-openapi.yml
consequence_counts:
  physical: 3
  read: 66
  safety-critical: 3
  write: 50
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Windows 10 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /geolocation/tracking
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /media/capture/sessions/{sessionId}/preview/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /media/capture/sessions/{sessionId}/video/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cortana/responses
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /networking/background-transfers/downloads
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /networking/http/requests
operation_count: 122
overview: 'Microsoft Windows 10 exposes 122 API operations that an AI agent could call, of which 56 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 66 read, 50 write, 3 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Windows 10
provider_slug: microsoft-windows-10
slug: microsoft-windows-10-agentic-access
source_filename: microsoft-windows-10-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-windows-10-background-tasks-openapi.yml, openapi/microsoft-windows-10-bluetooth-openapi.yml,\n  openapi/microsoft-windows-10-composition-openapi.yml, openapi/microsoft-windows-10-cortana-openapi.yml,\n  openapi/microsoft-windows-10-directx-openapi.yml, openapi/microsoft-windows-10-geolocation-openapi.yml,\n  openapi/microsoft-windows-10-hello-openapi.yml, openapi/microsoft-windows-10-ink-openapi.yml,\n  openapi/microsoft-windows-10-media-capture-openapi.yml, openapi/microsoft-windows-10-ml-openapi.yml,\n  openapi/microsoft-windows-10-networking-openapi.yml, openapi/microsoft-windows-10-notifications-openapi.yml,\n  openapi/microsoft-windows-10-sensors-openapi.yml, openapi/microsoft-windows-10-storage-openapi.yml,\n  openapi/microsoft-windows-10-win32-openapi.yml, openapi/microsoft-windows-10-winrt-openapi.yml,\n  openapi/microsoft-windows-10-winui-openapi.yml\ndescription: Recommended x-agentic-access execution\
  \ contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 122\n  by_action_class:\n    connected: 66\n    acting: 56\n  by_consequence:\n    read: 66\n    write: 50\n    physical: 3\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /background-tasks\n  method: get\n  operationId: listBackgroundTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /background-tasks\n  method: post\n  operationId: registerBackgroundTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /background-tasks/{taskId}\n  method: get\n  operationId: getBackgroundTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /background-tasks/{taskId}\n  method: delete\n  operationId: unregisterBackgroundTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /background-tasks/access\n  method: get\n  operationId: getBackgroundAccessStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /background-tasks/access\n  method: post\n  operationId: requestBackgroundAccess\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /background-tasks/triggers\n  method: get\n  operationId: listTriggerTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bluetooth/devices\n  method: get\n  operationId: listBluetoothDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bluetooth/devices/{deviceId}\n  method: get\n  operationId: getBluetoothDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bluetooth/le/scan\n  method: post\n  operationId: startBLEScan\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bluetooth/le/devices/{deviceId}/services\n  method: get\n  operationId: listGattServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bluetooth/le/devices/{deviceId}/services/{serviceId}/characteristics\n  method: get\n  operationId: listGattCharacteristics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bluetooth/le/devices/{deviceId}/services/{serviceId}/characteristics/{characteristicId}/value\n  method: get\n  operationId: readGattCharacteristic\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bluetooth/le/devices/{deviceId}/services/{serviceId}/characteristics/{characteristicId}/value\n  method: put\n  operationId: writeGattCharacteristic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bluetooth/rfcomm/connections\n  method: post\n  operationId: createRfcommConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /composition/visuals\n  method: get\n  operationId: listVisuals\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /composition/visuals\n  method: post\n  operationId: createVisual\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /composition/animations\n  method: post\n  operationId: createAnimation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /composition/effects\n  method: post\n  operationId: createEffect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /composition/surfaces\n  method: post\n  operationId: createSurface\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cortana/voice-commands\n  method: get\n  operationId: listVoiceCommandDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cortana/voice-commands\n  method: post\n  operationId: installVoiceCommandDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cortana/voice-commands/{commandSetName}\n  method: get\n  operationId: getVoiceCommandSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cortana/voice-commands/{commandSetName}/phrase-lists/{phraseListName}\n  method: put\n  operationId: updatePhraseList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cortana/service-connections\n  method: post\n  operationId: createCortanaServiceConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cortana/responses\n  method: post\n  operationId: sendCortanaResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /directx/devices\n  method: get\n  operationId: listDirectXDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directx/devices/{adapterId}\n  method: get\n  operationId: getDirectXDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /directx/resources\n  method: post\n  operationId: createDirectXResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /directx/command-queues\n  method: post\n  operationId: createCommandQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /directx/pipeline-states\n  method: post\n  operationId: createPipelineState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /directx/swap-chains\n  method: post\n  operationId: createSwapChain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geolocation/access\n  method: get\n  operationId: getGeolocationAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geolocation/access\n  method: post\n  operationId: requestGeolocationAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /geolocation/position\n  method: get\n  operationId: getCurrentPosition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geolocation/tracking\n  method: post\n  operationId: startPositionTracking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geolocation/tracking\n  method: delete\n  operationId: stopPositionTracking\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /geolocation/geofences\n  method: get\n  operationId: listGeofences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geolocation/geofences\n  method: post\n  operationId: createGeofence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geolocation/visits\n  method: get\n  operationId: getRecentVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hello/availability\n  method: get\n  operationId: checkHelloAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hello/credentials\n  method: post\n  operationId: createKeyCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hello/credentials/{accountId}\n  method: get\n  operationId: openKeyCredential\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hello/credentials/{accountId}\n  method: delete\n  operationId: deleteKeyCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /hello/sign\n  method: post\n  operationId: signWithCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hello/verify-user\n  method: post\n  operationId: verifyUserConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hello/attestation\n  method: get\n  operationId: getKeyAttestation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ink/strokes\n  method: get\n  operationId:\
  \ listInkStrokes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ink/strokes\n  method: post\n  operationId: addInkStroke\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ink/strokes/{strokeId}\n  method: get\n  operationId: getInkStroke\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ink/strokes/{strokeId}\n  method: delete\n  operationId: deleteInkStroke\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ink/recognize\n  method: post\n  operationId: recognizeInkStrokes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ink/recognizers\n  method: get\n  operationId: listInkRecognizers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ink/drawing-attributes\n  method: get\n  operationId: getDefaultDrawingAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ink/drawing-attributes\n  method: put\n  operationId: updateDefaultDrawingAttributes\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/capture/devices\n  method: get\n  operationId: listCaptureDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/capture/sessions\n  method: post\n  operationId: initializeMediaCapture\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/capture/sessions/{sessionId}/photo\n  method: post\n  operationId: capturePhoto\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/capture/sessions/{sessionId}/video/start\n  method: post\n  operationId: startVideoRecording\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/capture/sessions/{sessionId}/video/stop\n  method: post\n  operationId: stopVideoRecording\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /media/capture/sessions/{sessionId}/preview/start\n  method: post\n  operationId: startPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/capture/sessions/{sessionId}/preview/stop\n  method: post\n  operationId: stopPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ml/models\n  method: get\n  operationId: listMLModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /ml/models\n  method: post\n  operationId: loadMLModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ml/models/{modelId}\n  method: get\n  operationId: getMLModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ml/models/{modelId}\n  method: delete\n  operationId: unloadMLModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ml/sessions\n  method: post\n  operationId:\
  \ createMLSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ml/sessions/{sessionId}/evaluate\n  method: post\n  operationId: evaluateMLModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ml/devices\n  method: get\n  operationId: listMLDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networking/sockets/tcp\n  method: post\n  operationId: createTcpSocket\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networking/sockets/udp\n  method: post\n  operationId: createUdpSocket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networking/websockets\n  method: post\n  operationId: createWebSocket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networking/http/requests\n  method: post\n  operationId:\
  \ sendHttpRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networking/background-transfers/downloads\n  method: post\n  operationId: createBackgroundDownload\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /networking/background-transfers/downloads\n  method: get\n  operationId: listBackgroundDownloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /networking/connectivity\n  method: get\n  operationId: getNetworkConnectivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/toast\n  method: post\n  operationId: createToastNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications/toast\n  method: get\n  operationId: listToastNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/toast/{notificationTag}\n  method: get\n  operationId: getToastNotification\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/toast/{notificationTag}\n  method: delete\n  operationId: removeToastNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications/toast/scheduled\n  method: post\n  operationId: scheduleToastNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications/toast/scheduled\n  method: get\n  operationId: listScheduledToastNotifications\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/tile\n  method: post\n  operationId: updateTileNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications/badge\n  method: post\n  operationId: updateBadgeNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications/collections\n  method: get\n  operationId: listToastCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/collections\n  method: post\n  operationId: createToastCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sensors\n  method: get\n  operationId: listAvailableSensors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sensors/accelerometer/reading\n  method: get\n  operationId: getAccelerometerReading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sensors/gyrometer/reading\n  method: get\n  operationId: getGyrometerReading\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sensors/compass/reading\n  method: get\n  operationId: getCompassReading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sensors/inclinometer/reading\n  method: get\n  operationId: getInclinometerReading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sensors/light/reading\n  method: get\n  operationId: getLightSensorReading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sensors/barometer/reading\n  method: get\n  operationId: getBarometerReading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /sensors/orientation/reading\n  method: get\n  operationId: getOrientationReading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sensors/pedometer/reading\n  method: get\n  operationId: getPedometerReading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sensors/proximity/reading\n  method: get\n  operationId: getProximityReading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sensors/human-presence/reading\n  method: get\n  operationId: getHumanPresenceReading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/files\n\
  \  method: get\n  operationId: listStorageFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/files/{fileId}\n  method: get\n  operationId: getStorageFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/files/{fileId}\n  method: delete\n  operationId: deleteStorageFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/files/{fileId}/content\n  method: get\n  operationId: readFileContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /storage/files/{fileId}/content\n  method: put\n  operationId: writeFileContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/folders\n  method: get\n  operationId: listStorageFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/folders\n  method: post\n  operationId: createStorageFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/app-data/settings\n  method:\
  \ get\n  operationId: getAppSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/app-data/settings\n  method: put\n  operationId: updateAppSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/libraries\n  method: get\n  operationId: listStorageLibraries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/libraries/{libraryId}/changes\n  method: get\n  operationId: getLibraryChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /win32/api-categories\n  method: get\n  operationId: listWin32ApiCategories\n  x-agentic-access\n\n# --- truncated at 32 KB (35 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/agentic-access/microsoft-windows-10-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/agentic-access/microsoft-windows-10-agentic-access.yml
summary_line: 122 operations · 56 acting · 3 human-in-the-loop
tags:
- Desktop
- Operating System
- UWP
- Win32
- Windows
---
