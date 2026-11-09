---
acting_count: 97
action_class_counts:
  acting: 97
  connected: 78
api_specs:
- filename: easee-account-api-openapi.yml
  format: yaml
  label: Easee Account API
  slug: easee-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-account-api-openapi.yml
- filename: easee-authorizecharging-api-openapi.yml
  format: yaml
  label: Easee Authorize Charging API
  slug: easee-authorizecharging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-authorizecharging-api-openapi.yml
- filename: easee-charge-session-api-openapi.yml
  format: yaml
  label: Easee Charge Session API
  slug: easee-charge-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-charge-session-api-openapi.yml
- filename: easee-charger-api-openapi.yml
  format: yaml
  label: Easee Charger API
  slug: easee-charger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-charger-api-openapi.yml
- filename: easee-cloud-ocpp-api-openapi.yml
  format: yaml
  label: Easee Cloud OCPP API
  slug: easee-cloud-ocpp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-cloud-ocpp-api-openapi.yml
- filename: easee-daily-schedule-api-openapi.yml
  format: yaml
  label: Easee Daily schedule API
  slug: easee-daily-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-daily-schedule-api-openapi.yml
- filename: easee-delayed-schedule-api-openapi.yml
  format: yaml
  label: Easee Delayed schedule API
  slug: easee-delayed-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-delayed-schedule-api-openapi.yml
- filename: easee-direct-ocpp-for-operators-api-openapi.yml
  format: yaml
  label: Easee Direct OCPP - For Operators API
  slug: easee-direct-ocpp-for-operators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-direct-ocpp-for-operators-api-openapi.yml
- filename: easee-direct-ocpp-for-users-api-openapi.yml
  format: yaml
  label: Easee Direct OCPP - For Users API
  slug: easee-direct-ocpp-for-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-direct-ocpp-for-users-api-openapi.yml
- filename: easee-easeekeys-api-openapi.yml
  format: yaml
  label: Easee Easee Keys API
  slug: easee-easeekeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-easeekeys-api-openapi.yml
- filename: easee-energy-reporting-api-openapi.yml
  format: yaml
  label: Easee Energy Reporting API
  slug: easee-energy-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-energy-reporting-api-openapi.yml
- filename: easee-equalizer-api-openapi.yml
  format: yaml
  label: Easee Equalizer API
  slug: easee-equalizer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-equalizer-api-openapi.yml
- filename: easee-observations-api-openapi.yml
  format: yaml
  label: Easee Observations API
  slug: easee-observations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-observations-api-openapi.yml
- filename: easee-resources-api-openapi.yml
  format: yaml
  label: Easee Resources API
  slug: easee-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-resources-api-openapi.yml
- filename: easee-site-api-openapi.yml
  format: yaml
  label: Easee Site API
  slug: easee-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-site-api-openapi.yml
- filename: easee-site-charge-session-api-openapi.yml
  format: yaml
  label: Easee Site Charge Session API
  slug: easee-site-charge-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-site-charge-session-api-openapi.yml
- filename: easee-state-api-openapi.yml
  format: yaml
  label: Easee State API
  slug: easee-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-state-api-openapi.yml
- filename: easee-weekly-schedule-api-openapi.yml
  format: yaml
  label: Easee Weekly schedule API
  slug: easee-weekly-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easee/openapi/easee-weekly-schedule-api-openapi.yml
consequence_counts:
  physical: 54
  read: 78
  safety-critical: 12
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 12
kind: agentic-access
layout: agentic-access
method: generated
name: Easee Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/chargers/{chargerId}/commands/override_schedule
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/chargers/{chargerId}/commands/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/chargers/{chargerId}/commands/stop_charging
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/chargers/{chargerId}/schedules/daily/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/chargers/{chargerId}/schedules/delayed/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/chargers/{chargerId}/schedules/weekly/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/equalizers/{equalizerId}/commands/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/sites/{siteId}/easee-control-access/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/sites/{siteId}/easee-control-access/request
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /local-ocpp/v1/connections/chargers/{serialNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /local-ocpp/v1/operators/{operatorId}/connection-details
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /local-ocpp/v1/operators/{operatorId}/connections/chargers/{serialNumber}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/chargers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/accounts/chargers/{serial_no}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/chargers/lifetime-energy/{chargerId}/configure
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/chargers/{chargerId}/access
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/chargers/{chargerId}/access
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chargers/{chargerId}/basic_charge_plan
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/chargers/{chargerId}/basic_charge_plan
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chargers/{chargerId}/charge_schedule/features
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chargers/{chargerId}/commands/lock_state
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chargers/{chargerId}/commands/pause_charging
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chargers/{chargerId}/commands/resume_charging
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chargers/{chargerId}/commands/scan_wifi
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/chargers/{chargerId}/commands/set_dynamic_charger_current
operation_count: 175
overview: 'Easee exposes 175 API operations that an AI agent could call, of which 97 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 78 read, 31 write, 54 physical, and 12 safety-critical.


  12 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Easee
provider_slug: easee
slug: easee-agentic-access
source_filename: easee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/easee-cloud-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 175\n  by_action_class:\n    connected: 78\n    acting: 97\n  by_consequence:\n    read: 78\n    physical: 54\n    write: 31\n    safety-critical: 12\n  human_in_the_loop_required: 12\noperations:\n- path: /api/accounts/chargers\n  method: get\n  operationId: Account_GetChargerFavorites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/chargers\n  method: post\n  operationId: Account_AddChargerFavoriteByPin\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/chargers/{serial_no}\n  method: delete\n  operationId: Account_RemoveChargerFavorite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/easeekeys\n  method: get\n  operationId: EaseeKeys_GetEaseeKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/easeekeys\n  method: post\n  operationId: EaseeKeys_AddEaseeKey\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/easeekeys/{key}\n  method: put\n  operationId: EaseeKeys_UpdateEaseeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/easeekeys/{key}\n  method: delete\n  operationId: EaseeKeys_DeleteEaseeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/accounts/favorites\n  method: get\n  operationId: Account_GetFavorites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/login\n  method: post\n  operationId: Account_Authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/products\n  method: get\n  operationId: Account_GetProductFavorites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/profile\n  method: get\n  operationId: Account_GetProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/refresh_token\n  method: post\n  operationId: Account_RefreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{accountId}/invalidate_token\n  method: delete\n  operationId: Account_InvalidateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers\n  method: get\n  operationId: Charger_GetAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/chargers/lifetime-energy/{chargerId}/all\n  method: get\n  operationId: LifetimeEnergyReporting_GetChargerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/lifetime-energy/{chargerId}/configure\n  method: put\n  operationId: LifetimeEnergyReporting_Configure\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/lifetime-energy/{chargerId}/daily\n  method: get\n  operationId: LifetimeEnergyReporting_GetDailyForPeriod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/chargers/lifetime-energy/{chargerId}/hourly\n  method: get\n  operationId: LifetimeEnergyReporting_GetHourlyForPeriod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/lifetime-energy/{chargerId}/monthly\n  method: get\n  operationId: LifetimeEnergyReporting_GetMonthlyForPeriod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/lifetime-energy/{chargerId}/yearly\n  method: get\n  operationId: LifetimeEnergyReporting_GetYearlyForPeriod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}\n  method: get\n  operationId: Charger_GetChargerById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/access\n  method: put\n  operationId: Charger_SetChargerAccessLevel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/access\n  method: delete\n  operationId: Charger_LinkCharger\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/basic_charge_plan\n\
  \  method: get\n  operationId: Charger_GetChargePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/basic_charge_plan\n  method: post\n  operationId: Charger_AddChargePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/basic_charge_plan\n  method: delete\n  operationId: Charger_DeleteChargePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/charge_schedule/features\n  method: post\n  operationId: Charger_SetChargeScheduleFeatures\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/commands/lock_state\n  method: post\n  operationId: charger_set_cable_lock_state\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/commands/override_schedule\n\
  \  method: post\n  operationId: Charger_OverrideSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/chargers/{chargerId}/commands/pause_charging\n  method: post\n  operationId: Charger_PauseSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/commands/reboot\n  method: post\n  operationId: charger_reboot\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/chargers/{chargerId}/commands/resume_charging\n  method: post\n  operationId: Charger_ResumeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/commands/scan_wifi\n  method: post\n  operationId: charger_scan_wifi\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/commands/set_dynamic_charger_current\n  method: post\n  operationId: charger_set_dynamic_charger_current\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/commands/set_phase_mode\n  method: post\n  operationId: charger_set_phase_mode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/chargers/{chargerId}/commands/set_rfid_pairing_mode_async\n  method: post\n  operationId: charger_pair_rfid_tag\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/commands/set_wifi_config\n  method: post\n  operationId: charger_set_wifi_configuration\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/commands/smart_charging\n  method: post\n  operationId:\
  \ charger_enable_smart_charging\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/commands/start_charging\n  method: post\n  operationId: AuthorizeCharging_StartCharging\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/commands/stop_charging\n  method: post\n  operationId: charger_stop_charging\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/chargers/{chargerId}/commands/toggle_charging\n  method: post\n  operationId: Charger_ToggleCharging\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/commands/update_firmware\n  method: post\n  operationId: charger_update_firmware\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/config\n  method: get\n  operationId: Charger_GetCachedChargerConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/details\n  method: get\n  operationId: Charger_GetChargerDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/invitations\n  method: post\n  operationId: Charger_CreateChargerInvitationLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/invitations/{invitationId}\n  method: get\n  operationId: Charger_GetChargerInvitationPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/invitations/{invitationId}\n  method: delete\n  operationId: Charger_RemoveChargerInvitationLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/invitations/{invitationId}/accept\n  method: post\n  operationId: Charger_AcceptChargerInvitationLink\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/invitations/{invitationId}/resend_email\n  method: post\n  operationId: Charger_ResendChargerInvitationLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/pair\n  method: post\n  operationId: Charger_AddChargerToAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/partners\n  method: post\n  operationId: Charger_SetOperator\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/partners\n  method: get\n  operationId: Charger_GetChargerOperator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/partners/{partnerId}\n  method: delete\n  operationId: Charger_RemoveChargerOperator\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/permission\n  method: delete\n  operationId: Charger_DeleteUserChargerAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/permission\n  method: get\n  operationId: Charger_GetChargerUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/chargers/{chargerId}/schedules\n  method: get\n  operationId: GetChargersSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/schedules/daily\n  method: post\n  operationId: PostChargersSchedulesDaily\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/schedules/daily\n  method: get\n  operationId: GetChargersSchedulesDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/schedules/daily\n  method:\
  \ delete\n  operationId: DeleteChargersSchedulesDaily\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/schedules/daily/disable\n  method: post\n  operationId: PostChargersSchedulesDailyDisable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/chargers/{chargerId}/schedules/daily/enable\n  method: post\n  operationId: PostChargersSchedulesDailyEnable\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/schedules/delayed\n  method: post\n  operationId: PostChargersSchedulesDelayed\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/schedules/delayed\n  method: get\n  operationId: GetChargersSchedulesDelayed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/schedules/delayed\n\
  \  method: delete\n  operationId: DeleteChargersSchedulesDelayed\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/schedules/delayed/disable\n  method: post\n  operationId: PostChargersSchedulesDelayedDisable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/chargers/{chargerId}/schedules/delayed/enable\n  method: post\n  operationId: PostChargersSchedulesDelayedEnable\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/schedules/weekly\n  method: post\n  operationId: PostChargersSchedulesWeekly\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/schedules/weekly\n  method: get\n  operationId: GetChargersSchedulesWeekly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/chargers/{chargerId}/schedules/weekly\n  method: delete\n  operationId: DeleteChargersSchedulesWeekly\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/schedules/weekly/disable\n  method: post\n  operationId: PostChargersSchedulesWeeklyDisable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/chargers/{chargerId}/schedules/weekly/enable\n  method: post\n  operationId: PostChargersSchedulesWeeklyEnable\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/sessions/latest\n  method: get\n  operationId: Chargers_GetLastUpdatedChargeSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/sessions/ongoing\n  method: get\n  operationId: Chargers_GetOngoingSessionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/sessions/{sequenceId}\n  method: delete\n  operationId: Chargers_DeleteChargingSession\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/settings\n  method: post\n  operationId: Charger_SetChargerSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/site\n  method: get\n  operationId: Charger_GetChargerSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/unpair\n\
  \  method: post\n  operationId: Charger_RemoveChargerFromAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/usage/hourly/{from}/{to}\n  method: get\n  operationId: Charger_GetHourlyAggregatedUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/weekly_charge_plan\n  method: get\n  operationId: Charger_GetWeeklyChargeSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chargers/{chargerId}/weekly_charge_plan\n  method: post\n\
  \  operationId: Charger_AddWeeklyChargeSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chargers/{chargerId}/weekly_charge_plan\n  method: delete\n  operationId: Charger_DeleteWeeklyChargeSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cloud-ocpp/partners/{partnerId}\n  method: get\n  operationId: Partners_GetOcppConfig\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cloud-ocpp/partners/{partnerId}\n  method: post\n  operationId: Partners_SaveOcppConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cloud-ocpp/partners/{partnerId}/sites\n  method: get\n  operationId: Partners_GetAllCustomEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cloud-ocpp/partners/{partnerId}/sites/{siteId}\n  method: get\n  operationId: Partners_GetCustomEndpointsOnSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/cloud-ocpp/partners/{partnerId}/sites/{siteId}\n  method: post\n  operationId: Partners_SetCustomEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cloud-ocpp/partners/{partnerId}/sites/{siteId}\n  method: delete\n  operationId: Partners_DeleteCustomEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/equalizers/{equalizerId}\n  method: get\n  operationId: Equalizer_GetEqualizer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/equalizers/{equalizerId}/commands/configure_max_allocated_current\n  method: post\n  operationId: Equalizer_ConfigureAllocatedCurrent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/equalizers/{equalizerId}/commands/configure_meter_type\n  method: post\n  operationId: Equalizer_ConfigureMeterType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (58 KB total) ---\n# Full source: https://artifacts.apis.io/easee/agentic-access/easee-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/easee/agentic-access/easee-agentic-access.yml
summary_line: 175 operations · 97 acting · 12 human-in-the-loop
tags:
- Company
- EV Charging
- Smart Home
- IoT
- Energy
---
