---
acting_count: 54
action_class_counts:
  acting: 54
  connected: 11
api_specs:
- filename: tesla-openapi-original.yml
  format: yaml
  label: Tesla Fleet API
  slug: fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla/refs/heads/main/openapi/tesla-openapi-original.yml
- filename: tesla-openapi-original.yml
  format: yaml
  label: Tesla Owner API
  slug: owner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tesla/refs/heads/main/openapi/tesla-openapi-original.yml
consequence_counts:
  physical: 8
  read: 11
  safety-critical: 14
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 14
kind: agentic-access
layout: agentic-access
method: generated
name: Tesla Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/adjust_volume
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/auto_conditioning_stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/charge_stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/media_next_fav
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/media_next_track
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/media_prev_fav
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/media_prev_track
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/media_toggle_playback
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/media_volume_down
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/media_volume_up
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/reset_valet_pin
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/set_cabin_overheat_protection
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/sun_roof_control
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/window_control
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/charge_max_range
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/charge_port_door_close
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/charge_port_door_open
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/charge_standard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/charge_start
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/navigation_request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/set_charge_limit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/1/vehicles/{vehicle_id}/command/set_charging_amps
operation_count: 65
overview: 'Tesla exposes 65 API operations that an AI agent could call, of which 54 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 32 write, 8 physical, and 14 safety-critical.


  14 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tesla
provider_slug: tesla
slug: tesla-agentic-access
source_filename: tesla-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tesla-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 65\n  by_action_class:\n    acting: 54\n    connected: 11\n  by_consequence:\n    write: 32\n    read: 11\n    safety-critical: 14\n    physical: 8\n  human_in_the_loop_required: 14\noperations:\n- path: /oauth/token\n  method: post\n  operationId: CreateOauthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles\n  method: get\n  operationId: GetVehicles\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/vehicles/{vehicle_id}\n  method: get\n  operationId: GetVehicle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/vehicles/{vehicle_id}/mobile_enabled\n  method: get\n  operationId: GetVehicleMobileEnabled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/vehicles/{vehicle_id}/data_request/charge_state\n  method: get\n  operationId: GetVehicleChargeState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/vehicles/{vehicle_id}/data_request/climate_state\n  method: get\n  operationId: GetVehicleClimateState\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/vehicles/{vehicle_id}/data_request/drive_state\n  method: get\n  operationId: GetVehicleDriveState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/vehicles/{vehicle_id}/data_request/gui_settings\n  method: get\n  operationId: GetVehilceGuiSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/vehicles/{vehicle_id}/data_request/vehicle_state\n  method: get\n  operationId: GetVehicleState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/vehicles/{vehicle_id}/data_request/vehicle_config\n  method: get\n  operationId:\
  \ GetVehicleConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/vehicles/{vehicle_id}/vehicle_data\n  method: get\n  operationId: GetVehicleData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/vehicles/{vehicle_id}/wake_up\n  method: post\n  operationId: WakeUpVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/wake_up\n  method: post\n  operationId: WakeUpVehicleCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/set_valet_mode\n  method: post\n  operationId: ToggleValetMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/reset_valet_pin\n  method: post\n  operationId: ResetValetPin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/charge_port_door_open\n\
  \  method: post\n  operationId: OpenChargePort\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/charge_port_door_close\n  method: post\n  operationId: CloseChargePort\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/charge_standard\n  method: post\n  operationId: SendStandardChargeLimit\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/charge_max_range\n  method: post\n  operationId: SetMaxChargeLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/set_charge_limit\n  method: post\n  operationId: SetChargeLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n   \
  \   purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/set_charging_amps\n  method: post\n  operationId: SetChargingAmps\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/set_scheduled_departure\n  method: post\n  operationId: SetScheduledDeparture\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/1/vehicles/{vehicle_id}/command/set_scheduled_charging\n  method: post\n  operationId: SetScheduledCharging\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/charge_start\n  method: post\n  operationId: StartCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/charge_stop\n  method: post\n  operationId: StopCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/nearby_charging_sites\n  method: get\n  operationId: NearbyChargers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/vehicles/{vehicle_id}/command/flash_lights\n  method: post\n  operationId: FlashLights\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/honk_horn\n  method: post\n  operationId: HonkHorn\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/door_unlock\n  method: post\n  operationId: UnlockDoors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/door_lock\n  method: post\n  operationId: LockDoors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/1/vehicles/{vehicle_id}/command/set_temps\n  method: post\n  operationId: SetTemperatures\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/auto_conditioning_start\n  method: post\n  operationId: StartHVAC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/auto_conditioning_stop\n  method: post\n  operationId: StopHVAC\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/set_bioweapon_mode\n  method: post\n  operationId: BioweaponDefense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/set_climate_keeper_mode\n  method: post\n  operationId: ClimateKeeper\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/set_cabin_overheat_protection\n\
  \  method: post\n  operationId: CabinOverheatProtection\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/remote_seat_heater_request\n  method: post\n  operationId: RemoteSeatHeaterRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/remote_seat_cooler_request\n  method: post\n  operationId: RemoteSeatCoolerRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/remote_auto_seat_climate_request\n  method: post\n  operationId: RemoteAutoSeatClimateRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/remote_steering_wheel_heater_request\n  method: post\n  operationId: RemoteSteeringWheelHeaterRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/sun_roof_control\n  method: post\n  operationId: OpenSunroof\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/remote_start_drive\n  method: post\n  operationId: RemoteStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/actuate_trunk\n  method: post\n  operationId: OpenTrunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/speed_limit_activate\n  method: post\n  operationId: ActivateSpeedLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/speed_limit_deactivate\n  method: post\n  operationId: DeactivateSpeedLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/1/vehicles/{vehicle_id}/command/speed_limit_set_limit\n  method: post\n  operationId: SetSpeedLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/speed_limit_clear_pin\n  method: post\n  operationId: ClearSpeedLimitPin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/navigation_request\n  method: post\n  operationId: NavigationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/share\n  method: post\n  operationId: SharetoVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/media_toggle_playback\n  method: post\n  operationId: MediaTogglePlayback\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/media_next_track\n  method: post\n  operationId: MediaNextTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/media_prev_track\n  method: post\n  operationId: MediaPrevTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/media_next_fav\n  method: post\n  operationId: MediaNextFavorite\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/media_prev_fav\n  method: post\n  operationId: MediaPrevFavorite\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/media_volume_up\n  method: post\n  operationId: MediaVolumeUp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/media_volume_down\n  method: post\n  operationId: MediaVolumeDown\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/adjust_volume\n  method: post\n  operationId: MediaAdjustVolume\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/schedule_software_update\n\
  \  method: post\n  operationId: StartSoftwareUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/cancel_software_update\n  method: post\n  operationId: CancelSoftwareUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/set_sentry_mode\n  method: post\n  operationId: SetSentryMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/set_preconditioning_max\n  method: post\n  operationId: SetMaxDefrost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/window_control\n  method: post\n  operationId: WindowControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/trigger_homelink\n  method:\
  \ post\n  operationId: TriggerHomelink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/set_vehicle_name\n  method: post\n  operationId: SetVehicleName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/vehicles/{vehicle_id}/command/remote_boombox\n  method: post\n  operationId: RemoteBoombox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesla/refs/heads/main/agentic-access/tesla-agentic-access.yml
summary_line: 65 operations · 54 acting · 14 human-in-the-loop
tags:
- Automobiles
- Cars
- Vehicles
- Electric Vehicles
- Energy
- Clean Energy
- IoT
---
