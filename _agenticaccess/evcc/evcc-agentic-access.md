---
acting_count: 72
action_class_counts:
  acting: 72
  connected: 16
api_specs:
- filename: evcc-auth-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Auth API
  slug: evcc-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-auth-api-openapi.yml
- filename: evcc-battery-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Battery API
  slug: evcc-battery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-battery-api-openapi.yml
- filename: evcc-db-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Db API
  slug: evcc-db-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-db-api-openapi.yml
- filename: evcc-experimental-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Experimental API
  slug: evcc-experimental-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-experimental-api-openapi.yml
- filename: evcc-general-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) General API
  slug: evcc-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-general-api-openapi.yml
- filename: evcc-loadpoints-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Loadpoints API
  slug: evcc-loadpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-loadpoints-api-openapi.yml
- filename: evcc-sessions-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Sessions API
  slug: evcc-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-sessions-api-openapi.yml
- filename: evcc-state-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) State API
  slug: evcc-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-state-api-openapi.yml
- filename: evcc-system-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) System API
  slug: evcc-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-system-api-openapi.yml
- filename: evcc-tariffs-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Tariffs API
  slug: evcc-tariffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-tariffs-api-openapi.yml
- filename: evcc-vehicles-api-openapi.yml
  format: yaml
  label: evcc (self-hosted) Vehicles API
  slug: evcc-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evcc/openapi/evcc-vehicles-api-openapi.yml
consequence_counts:
  physical: 8
  read: 16
  safety-critical: 10
  write: 54
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Evcc Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /batterydischargecontrol/{enable}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /batterygriddischarge/{enable}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /batterymode
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /db/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /loadpoints/{id}/disable/delay/{delay}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /loadpoints/{id}/disable/threshold/{threshold}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /settings/telemetry/{enable}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /system/shutdown
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /vehicles/{name}/alwayscharge
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /vehicles/{name}/mode
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /batterygridchargelimit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /batterygridchargelimit/{cost}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /batterygriddischargelimit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /batterygriddischargelimit/{cost}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /loadpoints/{id}/alwayscharge/{alwaysCharge}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /loadpoints/{id}/mode/{mode}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vehicles/{name}/alwayscharge/{alwaysCharge}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vehicles/{name}/mode/{mode}
operation_count: 88
overview: 'evcc (self-hosted) exposes 88 API operations that an AI agent could call, of which 72 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 54 write, 8 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: evcc (self-hosted)
provider_slug: evcc
slug: evcc-agentic-access
source_filename: evcc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/evcc-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 88\n  by_action_class:\n    acting: 72\n    connected: 16\n  by_consequence:\n    write: 54\n    read: 16\n    safety-critical: 10\n    physical: 8\n  human_in_the_loop_required: 10\noperations:\n- path: /auth/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/password\n  method: put\n  operationId: changePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/status\n  method: get\n  operationId: getAuthStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/apikey\n  method: get\n  operationId: getApiKeyStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /auth/apikey\n  method: post\n  operationId: regenerateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batterydischargecontrol/{enable}\n  method: post\n  operationId: setBatteryDischargeControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /batterygriddischarge/{enable}\n  method: post\n  operationId: setBatteryGridDischarge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /batterygridchargelimit\n  method: delete\n  operationId: removeBatteryGridChargeLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batterygridchargelimit/{cost}\n  method: post\n  operationId: setBatteryGridChargeLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /batterygriddischargelimit\n  method: delete\n  operationId: removeBatteryGridDischargeLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batterygriddischargelimit/{cost}\n  method: post\n  operationId: setBatteryGridDischargeLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batterymode\n  method: delete\n  operationId: disableExternalBatteryControl\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /batterymode/{batteryMode}\n  method: post\n  operationId: setExternalBatteryMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buffersoc/{soc}\n  method: post\n  operationId: setBufferSoc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /bufferstartsoc/{soc}\n  method: post\n  operationId: setBufferStartSoc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/alwayscharge/{alwaysCharge}\n  method: post\n  operationId: setLoadpointAlwaysCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/batteryboost/{enable}\n  method: post\n  operationId: setLoadpointBatteryBoost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/batteryboostlimit/{soc}\n  method: post\n  operationId: setLoadpointBatteryBoostLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/disable/delay/{delay}\n  method: post\n  operationId: setLoadpointDisableDelay\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /loadpoints/{id}/disable/threshold/{threshold}\n  method: post\n  operationId: setLoadpointDisableThreshold\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /loadpoints/{id}/enable/delay/{delay}\n  method: post\n  operationId: setLoadpointEnableDelay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/enable/threshold/{threshold}\n  method: post\n  operationId: setLoadpointEnableThreshold\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/limitenergy/{energy}\n  method: post\n  operationId: setLoadpointEnergyLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/limitsoc/{soc}\n  method: post\n  operationId: setLoadpointSocLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/maxcurrent/{current}\n\
  \  method: post\n  operationId: setLoadpointMaxCurrent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/mincurrent/{current}\n  method: post\n  operationId: setLoadpointMinCurrent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/mintemp/{temp}\n  method: post\n  operationId: setLoadpointMinTemp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/mode/{mode}\n  method: post\n  operationId: setLoadpointMode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/phases/{phases}\n  method: post\n  operationId: setLoadpointPhases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/plan\n  method: get\n  operationId: getLoadpointPlan\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loadpoints/{id}/plan/energy\n  method: delete\n  operationId: deleteLoadpointEnergyPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/plan/energy/{energy}/{timestamp}\n  method: post\n  operationId: setLoadpointEnergyPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/plan/repeating/preview/{soc}/{weekdays}/{hourMinuteTime}/{timezone}\n  method: get\n  operationId: previewLoadpointRepeatingPlan\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loadpoints/{id}/plan/static/preview/soc/{soc}/{timestamp}\n  method: get\n  operationId: previewLoadpointSocPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loadpoints/{id}/plan/static/preview/energy/{energy}/{timestamp}\n  method: get\n  operationId: previewLoadpointEnergyPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loadpoints/{id}/plan/strategy\n  method: post\n  operationId: setLoadpointPlanStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/priority/{priority}\n  method: post\n  operationId: setLoadpointPriority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/smartcostlimit\n  method: delete\n  operationId: deleteLoadpointSmartCostLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/smartcostlimit/{cost}\n  method: post\n  operationId: setLoadpointSmartCostLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/smartfeedinprioritylimit\n  method: delete\n  operationId: deleteLoadpointSmartFeedInPriorityLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/smartfeedinprioritylimit/{cost}\n  method: post\n  operationId: setLoadpointSmartFeedInPriorityLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /loadpoints/{id}/solarshare/{share}\n  method: post\n  operationId: setLoadpointSolarShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/vehicle\n  method: delete\n  operationId: removeLoadpointVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/vehicle\n  method: patch\n  operationId: startLoadpointVehicleDetection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loadpoints/{id}/vehicle/{name}\n  method: post\n  operationId: assignLoadpointVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prioritysoc/{soc}\n  method: post\n  operationId: setPrioritySoc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /residualpower/{power}\n  method: post\n  operationId: setResidualPower\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gridexportlimit/{power}\n  method: post\n  operationId: setGridExportLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /solaradjusted/{enable}\n  method: post\n  operationId: setSolarAdjusted\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config/optimizerautomatic/{value}\n  method: post\n  operationId:\
  \ setOptimizerAutomatic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config/onboarding\n  method: put\n  operationId: setOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smartfeedinprioritylimit\n  method: delete\n  operationId: removeGlobalSmartFeedInPriorityLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /smartfeedinprioritylimit/{cost}\n  method: post\n  operationId: setGlobalSmartFeedInPriorityLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session/{id}\n  method: put\n  operationId: updateSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session/{id}\n  method: delete\n  operationId: deleteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gridsessions\n  method: get\n  operationId: getGridSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: get\n  operationId: getSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config/currency\n  method: put\n  operationId: setCurrency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config/country\n  method: put\n  operationId: setCountry\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config/gridconnection\n  method: put\n  operationId: setGridConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/telemetry/{enable}\n  method: post\n  operationId: setTelemetryStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /smartcostlimit\n  method: delete\n  operationId: removeGlobalSmartCostLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smartcostlimit/{cost}\n  method: post\n  operationId: setGlobalSmartCostLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /state\n  method: get\n  operationId: getState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/log\n  method: get\n  operationId: getSystemLogs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/log/areas\n  method: get\n  operationId: getLogAreas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/cache\n  method: delete\n  operationId: clearCache\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /system/shutdown\n  method: post\n  operationId: shutdownSystem\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tariff/{type}\n  method: get\n  operationId: getTariffInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles/{name}/limitsoc/{soc}\n  method: post\n  operationId: setVehicleSocLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicles/{name}/minsoc/{soc}\n  method: post\n  operationId: setVehicleMinSoc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /vehicles/{name}/mode\n  method: delete\n  operationId: deleteVehicleMode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /vehicles/{name}/mode/{mode}\n  method: post\n  operationId: setVehicleMode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicles/{name}/alwayscharge\n  method: delete\n  operationId: deleteVehicleAlwaysCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /vehicles/{name}/alwayscharge/{alwaysCharge}\n  method: post\n  operationId: setVehicleAlwaysCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicles/{name}/plan/repeating\n  method: post\n  operationId: updateVehicleRepeatingPlans\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /vehicles/{name}/plan/soc\n  method: delete\n  operationId: deleteVehicleSocPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicles/{name}/plan/soc/{soc}/{timestamp}\n  method: post\n  operationId: setVehicleSocPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vehicles/{name}/plan/strategy\n  method: post\n  operationId: setVehiclePlanStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/backup\n  method: get\n  operationId: downloadBackup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /db/restore\n  method: post\n  operationId: restoreBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/reset\n  method: post\n  operationId: resetDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /db/metrics/energy\n  method: delete\n  operationId: deleteEnergyMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /db/metrics/tariffs\n  method: delete\n  operationId: deleteTariffMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /history/energy\n  method: get\n  operationId: getEnergyHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /history/flow\n  method: get\n  operationId: getEnergyFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/tariffs\n  method: get\n  operationId: getTariffHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/evcc/agentic-access/evcc-agentic-access.yml
summary_line: 88 operations · 72 acting · 10 human-in-the-loop
tags:
- Company
- Electric Vehicles
- Smart Charging
- Open Source
- Energy Management
- Home Automation
---
