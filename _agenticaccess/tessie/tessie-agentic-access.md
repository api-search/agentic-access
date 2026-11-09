---
acting_count: 67
action_class_counts:
  acting: 67
  connected: 25
api_specs:
- filename: tessie-driver-management-api-openapi.yml
  format: yaml
  label: Tessie Driver Management API
  slug: tessie-driver-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-driver-management-api-openapi.yml
- filename: tessie-telemetry-configuration-api-openapi.yml
  format: yaml
  label: Tessie Telemetry Configuration API
  slug: tessie-telemetry-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-telemetry-configuration-api-openapi.yml
- filename: tessie-vehicle-commands-api-openapi.yml
  format: yaml
  label: Tessie Vehicle Commands API
  slug: tessie-vehicle-commands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-vehicle-commands-api-openapi.yml
- filename: tessie-vehicle-data-api-openapi.yml
  format: yaml
  label: Tessie Vehicle Data API
  slug: tessie-vehicle-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessie/openapi/tessie-vehicle-data-api-openapi.yml
consequence_counts:
  physical: 6
  read: 25
  safety-critical: 11
  write: 50
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 11
kind: agentic-access
layout: agentic-access
method: generated
name: Tessie Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{vin}/command/disable_guest
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{vin}/command/disable_keep_accessory_power_mode
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{vin}/command/disable_low_power_mode
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{vin}/command/disable_sentry
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{vin}/command/disable_speed_limit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{vin}/command/disable_valet
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{vin}/command/stop_charging
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{vin}/command/stop_climate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{vin}/command/stop_max_defrost
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{vin}/command/stop_steering_wheel_heater
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{vin}/invitations/{id}/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{vin}/charges/{id}/set_cost
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{vin}/command/add_charge_schedule
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{vin}/command/close_charge_port
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{vin}/command/open_charge_port
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{vin}/command/remove_charge_schedule
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{vin}/command/set_charge_limit
operation_count: 92
overview: 'Tessie exposes 92 API operations that an AI agent could call, of which 67 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 50 write, 6 physical, and 11 safety-critical.


  11 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tessie
provider_slug: tessie
slug: tessie-agentic-access
source_filename: tessie-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/tessie-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 92\n  by_action_class:\n    connected: 25\n    acting: 67\n  by_consequence:\n    read: 25\n    write: 50\n    physical: 6\n    safety-critical: 11\n  human_in_the_loop_required: 11\noperations:\n- path: /{vin}/state\n  method: get\n  operationId: get-state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vehicles\n  method: get\n  operationId: get-vehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/states\n\
  \  method: get\n  operationId: get-historical-states\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/battery\n  method: get\n  operationId: get-battery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /battery_health\n  method: get\n  operationId: get-battery-health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/battery_health\n  method: get\n  operationId: get-battery-health-measurements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/location\n  method: get\n  operationId: get-location\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/firmware_alerts\n  method: get\n  operationId: get-firmware-alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/release_notes/{version}\n  method: get\n  operationId: get-release-notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/map\n  method: get\n  operationId: get-map\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/consumption_since_charge\n  method: get\n  operationId: get-consumption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/weather\n\
  \  method: get\n  operationId: get-weather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/drives\n  method: get\n  operationId: get-drives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/path\n  method: get\n  operationId: get-driving-path\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/drives/set_tag\n  method: post\n  operationId: set-drive-tag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/charges\n  method:\
  \ get\n  operationId: get-charges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /charging_invoices\n  method: get\n  operationId: get-fleet-charging-invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/charges/{id}/set_cost\n  method: post\n  operationId: set-charge-cost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/idles\n  method: get\n  operationId: get-idles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /{vin}/last_idle_state\n  method: get\n  operationId: get-last-idle-state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/tire_pressure\n  method: get\n  operationId: get-tire-pressure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/status\n  method: get\n  operationId: get-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/wake\n  method: post\n  operationId: wake\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /{vin}/command/lock\n  method: post\n  operationId: lock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/unlock\n  method: post\n  operationId: unlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/activate_front_trunk\n  method: post\n  operationId: activate-front-trunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/activate_rear_trunk\n  method: post\n  operationId: activate-rear-trunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/open_tonneau\n  method: post\n  operationId: open-tonneau\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/close_tonneau\n  method: post\n  operationId: close-tonneau\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/vent_windows\n  method: post\n  operationId: vent-windows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/close_windows\n  method: post\n  operationId: close-windows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/start_climate\n  method: post\n  operationId: start-climate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/stop_climate\n  method: post\n  operationId: stop-climate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{vin}/command/set_temperatures\n  method: post\n  operationId: set-temperatures\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /{vin}/command/set_seat_heat\n  method: post\n  operationId: set-seat-heating\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/set_seat_cool\n  method: post\n  operationId: set-seat-cooling\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/start_max_defrost\n  method: post\n  operationId: start-max-defrost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/stop_max_defrost\n  method: post\n  operationId: stop-max-defrost\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{vin}/command/start_steering_wheel_heater\n  method: post\n  operationId: start-steering-wheel-heater\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/stop_steering_wheel_heater\n  method: post\n  operationId: stop-steering-wheel-heater\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{vin}/command/set_cabin_overheat_protection\n  method: post\n  operationId: set-cabin-overheat-protection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/set_cop_temp\n  method: post\n  operationId: set-cabin-overheat-protection-temp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/set_bioweapon_mode\n  method: post\n  operationId: set-bioweapon-mode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/set_climate_keeper_mode\n  method: post\n  operationId: set-climate-keeper-mode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/start_charging\n  method: post\n  operationId: start-charging\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/stop_charging\n  method: post\n  operationId: stop-charging\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{vin}/command/set_charge_limit\n  method: post\n  operationId: set-charge-limit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /{vin}/command/set_charging_amps\n  method: post\n  operationId: set-charging-amps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/open_charge_port\n  method: post\n  operationId: open-charge-port\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/close_charge_port\n  method: post\n  operationId: close-charge-port\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/flash\n  method: post\n  operationId: flash\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/honk\n  method: post\n  operationId: honk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/trigger_homelink\n  method: post\n  operationId: trigger-homelink\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/remote_start\n  method: post\n  operationId: remote-start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/vent_sunroof\n  method: post\n  operationId: vent-sunroof\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /{vin}/command/close_sunroof\n  method: post\n  operationId: close-sunroof\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/enable_sentry\n  method: post\n  operationId: enable-sentry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/disable_sentry\n  method: post\n  operationId: disable-sentry\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{vin}/command/enable_valet\n  method: post\n  operationId: enable-valet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/disable_valet\n  method: post\n  operationId: disable-valet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{vin}/command/enable_low_power_mode\n  method: post\n  operationId: enable-low-power\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/disable_low_power_mode\n  method: post\n  operationId: disable-low-power\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{vin}/command/enable_keep_accessory_power_mode\n  method: post\n  operationId: enable-keep-accessory-power\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /{vin}/command/disable_keep_accessory_power_mode\n  method: post\n  operationId: disable-keep-accessory-power\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{vin}/command/schedule_software_update\n  method: post\n  operationId: schedule-software-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/cancel_software_update\n  method: post\n  operationId: cancel-software-update\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/set_scheduled_charging\n  method: post\n  operationId: set-scheduled-charging\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/set_scheduled_departure\n  method: post\n  operationId: set-scheduled-departure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/add_charge_schedule\n\
  \  method: post\n  operationId: add-charge-schedule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/remove_charge_schedule\n  method: post\n  operationId: Remove-charge-schedule\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/add_precondition_schedule\n  method: post\n  operationId: add-precondition-schedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/remove_precondition_schedule\n  method: post\n  operationId: remove-precondition-schedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/share\n  method: post\n  operationId: share\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/remote_boombox\n  method: post\n  operationId:\
  \ boombox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/set_speed_limit\n  method: post\n  operationId: set-speed-limit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/enable_speed_limit\n  method: post\n  operationId: enable-speed-limit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /{vin}/command/disable_speed_limit\n  method: post\n  operationId: disable-speed-limit\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{vin}/command/clear_speed_limit_pin\n  method: post\n  operationId: clear-speed-limit-pin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/drivers\n  method: get\n  operationId: get-drivers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /{vin}/drivers/{id}/delete\n  method: post\n  operationId: delete-driver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/enable_guest\n  method: post\n  operationId: enable-guest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/command/disable_guest\n  method: post\n  operationId: disable-guest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n \
  \     purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{vin}/roles\n  method: get\n  operationId: get-roles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/roles\n  method: post\n  operationId: set-roles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/invitations\n  method: get\n  operationId: get-invitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/invitations\n  method: post\n  operationId: create-invitation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/invitations/{id}/revoke\n  method: post\n  operationId: revoke-invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{vin}/plate\n  method: get\n  operationId: get-plate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/plate\n  method: post\n  operationId: set-plate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/fleet_telemetry_config\n  method: get\n  operationId: get-fleet-telemetry-config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vin}/fleet_telemetry_config\n  method: post\n  operationId: set-fleet-telemetry-config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{vin}/fleet_telemetry_config\n  method: delete\n  operationId: delete-fleet-telemetry-config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/tessie/agentic-access/tessie-agentic-access.yml
summary_line: 92 operations · 67 acting · 11 human-in-the-loop
tags:
- Company
- Tesla
- Fleet Management
- Automotive
---
