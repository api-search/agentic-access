---
acting_count: 89
action_class_counts:
  acting: 89
  connected: 1
api_specs:
- filename: opkey-apk-instrumentation-api-openapi.yml
  format: yaml
  label: Opkey Apk Instrumentation API
  slug: opkey-apk-instrumentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-apk-instrumentation-api-openapi.yml
- filename: opkey-apk-instrumentation-apis-api-openapi.yml
  format: yaml
  label: Opkey Apk Instrumentation Apis API
  slug: opkey-apk-instrumentation-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-apk-instrumentation-apis-api-openapi.yml
- filename: opkey-app-center-api-api-openapi.yml
  format: yaml
  label: Opkey App Center Api API
  slug: opkey-app-center-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-app-center-api-api-openapi.yml
- filename: opkey-app-control-api-openapi.yml
  format: yaml
  label: Opkey App Control API
  slug: opkey-app-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-app-control-api-openapi.yml
- filename: opkey-appium-automation-api-openapi.yml
  format: yaml
  label: Opkey Appium Automation API
  slug: opkey-appium-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-appium-automation-api-openapi.yml
- filename: opkey-authentication-api-openapi.yml
  format: yaml
  label: Opkey Authentication API
  slug: opkey-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-authentication-api-openapi.yml
- filename: opkey-device-booking-session-api-openapi.yml
  format: yaml
  label: Opkey Device Booking & Session API
  slug: opkey-device-booking-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-device-booking-session-api-openapi.yml
- filename: opkey-device-interaction-api-openapi.yml
  format: yaml
  label: Opkey Device Interaction API
  slug: opkey-device-interaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-device-interaction-api-openapi.yml
- filename: opkey-file-management-api-openapi.yml
  format: yaml
  label: Opkey File Management API
  slug: opkey-file-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-file-management-api-openapi.yml
- filename: opkey-generic-api-openapi.yml
  format: yaml
  label: Opkey Generic API
  slug: opkey-generic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-generic-api-openapi.yml
- filename: opkey-network-simulation-api-openapi.yml
  format: yaml
  label: Opkey Network Simulation API
  slug: opkey-network-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-network-simulation-api-openapi.yml
- filename: opkey-performance-api-openapi.yml
  format: yaml
  label: Opkey Performance API
  slug: opkey-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-performance-api-openapi.yml
- filename: opkey-resigning-apis-api-openapi.yml
  format: yaml
  label: Opkey Resigning Apis API
  slug: opkey-resigning-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-resigning-apis-api-openapi.yml
- filename: opkey-session-media-logs-api-openapi.yml
  format: yaml
  label: Opkey Session Media & Logs API
  slug: opkey-session-media-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-session-media-logs-api-openapi.yml
- filename: opkey-xctest-automation-api-openapi.yml
  format: yaml
  label: Opkey Xctest Automation API
  slug: opkey-xctest-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-xctest-automation-api-openapi.yml
consequence_counts:
  physical: 2
  read: 1
  safety-critical: 6
  write: 81
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Opkey Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/check-app-installed
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/close-app
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/generic/kill-app
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/install-app
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/networkshaping/stop-throttle
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/open-app
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/send-home
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/send-text
operation_count: 90
overview: 'Opkey exposes 90 API operations that an AI agent could call, of which 89 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 81 write, 2 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Opkey
provider_slug: opkey
slug: opkey-agentic-access
source_filename: opkey-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/opkey-pcloudy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 90\n  by_action_class:\n    connected: 1\n    acting: 89\n  by_consequence:\n    read: 1\n    safety-critical: 6\n    write: 81\n    physical: 2\n  human_in_the_loop_required: 6\noperations:\n- path: /api/access\n  method: get\n  operationId: authentication2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/generic/kill-app\n  method: post\n  operationId: killApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/generic/uninstall-app\n  method: post\n  operationId: uninstallApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/generic/geo-ip-location\n  method: post\n  operationId: geoIpLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/generic/init-liveview\n  method: post\n  operationId: startStreamer\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/generic/set-location\n  method: post\n  operationId: setLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/generic/set-timezone\n  method: post\n  operationId: setTimezone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/download/session-video\n\
  \  method: post\n  operationId: downloadSessionVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/device-logs-download\n  method: post\n  operationId: deviceLogsDownload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/video-record\n  method: post\n  operationId: enableVideoRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/crash-logs-download\n  method: post\n  operationId: crashLogsDownload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/session-video/upload-progress\n  method: post\n  operationId: videoUploadProgress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/check-app-installed\n  method: post\n  operationId: checkAppInstalled\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/install-app\n  method: post\n  operationId: installApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/start-transaction\n  method: post\n  operationId: startTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/start_performance_data\n  method: post\n \
  \ operationId: startPerformance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/manual_access_files_list\n  method: post\n  operationId: performanceFileList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/download_manual_access_data\n  method: post\n  operationId: downloadPerformance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v2/send-text\n  method: post\n  operationId: sendText\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/rotate-device\n  method: post\n  operationId: rotateDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/send-home\n  method: post\n  operationId: sendHome\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/execute-adb\n  method: post\n  operationId: executeAdb\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/set-passcode\n  method: post\n  operationId: setPasscodeIos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/toggle-offline-mode\n  method: post\n  operationId: toggleOfflineModeEnable\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fingerprint_auth\n  method: post\n  operationId: biometricAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/imageInject\n  method: post\n  operationId: injectImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/install_app\n  method:\
  \ post\n  operationId: installLaunchApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/open-app\n  method: post\n  operationId: openApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/close-app\n  method: post\n  operationId: closeApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/lonelyappium\n  method: post\n  operationId: lonelyappium\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/appium/init\n  method: post\n  operationId: bookDevicesAppium\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/appium/execute\n  method: post\n  operationId: initAppiumhub\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/appium/get_appium_file_list\n  method: post\n  operationId: getAppiumFileList2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/appium/update_session\n  method: post\n  operationId: updateAppiumSession2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/appium/download_appium_access_data\n  method: post\n  operationId: downloadAppiumPerf\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /https://device.pcloudy.com/appium/wd/hub/session\n  method: post\n  operationId: appiumSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/automationbooking\n  method: post\n  operationId: xctestBookDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/xctest/initiate\n\
  \  method: post\n  operationId: xctestInitAutomation2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/xctest/start_device_services\n  method: post\n  operationId: xctestStartServices2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/getAutomationShareableLink\n  method: post\n  operationId: xctestShareableLink2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/xctest/release_devices\n  method: post\n  operationId: xctestReleaseDevices2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/networkshaping/start-throttle\n  method: post\n  operationId: startNetworkSimulation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/networkshaping/stop-throttle\n  method: post\n  operationId: stopNetworkSimulation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/filesinfo\n  method: post\n  operationId: filesInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/upload\n  method: post\n  operationId: uploadApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pushFileToSwapBox\n  method: post\n  operationId: pushFile2\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/delete_file\n  method: post\n  operationId: deleteFileCloud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/clean-device\n  method: post\n  operationId: cleanDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/release-device\n\
  \  method: post\n  operationId: releaseDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/devices\n  method: post\n  operationId: getDeviceList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/startdeviceservices\n  method: post\n  operationId: startDeviceServices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/book_device\n  method: post\n  operationId: bookDevice2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/release_device\n  method: post\n  operationId: releaseDevice2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/app_instrumentation/initiate\n  method: post\n  operationId: instrumentInitiate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/app_instrumentation/progress\n  method: post\n  operationId: instrumentationProgress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/app_instrumentation/download-to-cloud-drive\n  method: post\n  operationId: downloadInstrumentedFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/resign/initiate\n  method: post\n  operationId: initiateResigning\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/resign/progress\n  method: post\n  operationId: resigningProgress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/resign/download\n  method: post\n  operationId: downloadResigned\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get_user_details\n  method: post\n  operationId: getUserDetails\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/upload_file\n  method: post\n  operationId: uploadApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/drive\n  method: post\n  operationId: getAvailableApps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/download_file\n  method:\
  \ post\n  operationId: downloadFileCloud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get_devices_details\n  method: post\n  operationId: getSingleDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get_device_url\n  method: post\n  operationId: getDevicePageUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /api/execute_adb\n  method: post\n  operationId: executeAdb2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/wifi_statehandler\n  method: post\n  operationId: toggleWifi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/set_deviceLocation\n  method: post\n  operationId: setLocation2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/capture_device_screenshot\n  method: post\n  operationId: captureScreenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get_device_sessionDetails\n  method: post\n  operationId: sessionDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/wildnet\n  method: post\n  operationId: wildnet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/start_device_services\n  method: post\n  operationId: startDeviceServices2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/qr_image_inject\n  method: post\n  operationId: qrImageInject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/biometric_authentication\n  method: post\n  operationId: biometricAuth\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/instrument/initiate\n  method: post\n  operationId: instrumentInitiate2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/instrument/progress\n  method: post\n  operationId: instrumentationProgress2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/instrument/download\n\
  \  method: post\n  operationId: downloadInstrumented\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/appium/devices\n  method: post\n  operationId: bookDevicesAppium2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/appium/endpoint\n  method: post\n  operationId: getAppiumEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/appium/folder\n  method: post\n  operationId: getAppiumReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/appium/getShareableReportLink\n  method: post\n  operationId: appiumShareableLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/xctest/book_devices\n  method: post\n  operationId: xctestBookDevices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get_atcd_profiles\n  method: post\n  operationId: getNetworkProfiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/atcd_shape\n  method: post\n  operationId: setNetworkProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/atcd_unshape\n  method: post\n  operationId: unshapeNetwork\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get_appcenter_apps\n  method: post\n  operationId: getAppCenterApps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get_appcenter_app_releases\n  method: post\n  operationId: appCenterReleases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/get_appcenter_app_release_details\n  method: post\n  operationId:\
  \ appCenterReleaseDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/upload_appcenter_app\n  method: post\n  operationId: downloadUploadAppCenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/delete_external_app\n  method: post\n  operationId: deleteAppCenterApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/agentic-access/opkey-agentic-access.yml
summary_line: 90 operations · 89 acting · 6 human-in-the-loop
tags:
- Company
- Testing
- Test Automation
- Quality Assurance
- DevOps
- Continuous Integration
- Mobile Testing
- Device Cloud
- ERP
- Artificial Intelligence
- Agents
- MCP
---
