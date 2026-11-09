---
acting_count: 90
action_class_counts:
  acting: 90
  connected: 91
api_specs:
- filename: calc-engineer-auth-api-openapi.yml
  format: yaml
  label: calc.engineer Auth API
  slug: calc-engineer-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-auth-api-openapi.yml
- filename: calc-engineer-catalog-api-openapi.yml
  format: yaml
  label: calc.engineer Catalog API
  slug: calc-engineer-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-catalog-api-openapi.yml
- filename: calc-engineer-docs-api-openapi.yml
  format: yaml
  label: calc.engineer Docs API
  slug: calc-engineer-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-docs-api-openapi.yml
- filename: calc-engineer-general-api-openapi.yml
  format: yaml
  label: calc.engineer General API
  slug: calc-engineer-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-general-api-openapi.yml
- filename: calc-engineer-homelab-api-openapi.yml
  format: yaml
  label: calc.engineer Homelab API
  slug: calc-engineer-homelab-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-homelab-api-openapi.yml
- filename: calc-engineer-mesh-api-openapi.yml
  format: yaml
  label: calc.engineer Mesh API
  slug: calc-engineer-mesh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-mesh-api-openapi.yml
- filename: calc-engineer-pcb-api-openapi.yml
  format: yaml
  label: calc.engineer Pcb API
  slug: calc-engineer-pcb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-pcb-api-openapi.yml
- filename: calc-engineer-power-api-openapi.yml
  format: yaml
  label: calc.engineer Power API
  slug: calc-engineer-power-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-power-api-openapi.yml
- filename: calc-engineer-rf-api-openapi.yml
  format: yaml
  label: calc.engineer Rf API
  slug: calc-engineer-rf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-rf-api-openapi.yml
consequence_counts:
  physical: 24
  read: 91
  safety-critical: 13
  write: 53
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 13
kind: agentic-access
layout: agentic-access
method: generated
name: Calc Engineer Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/battery_charge_time
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/capacitor_charge
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/confidence_interval
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/inverter_sizing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/keys/{prefix}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/meshtastic_power
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/meshtastic_range
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/microstrip
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/solar_load_audit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/solar_sizing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/spice_simulate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/string_sizing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ups_runtime
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/battery_autonomy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/battery_life
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/channel_utilization
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/date_difference
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/eirp_compliance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/generator_offset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/impedance_match
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/link_budget
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/loan_amortization
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/log_calc
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/lora_param_optimizer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/lora_range_estimate
operation_count: 181
overview: 'calc.engineer exposes 181 API operations that an AI agent could call, of which 90 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 91 read, 53 write, 24 physical, and 13 safety-critical.


  13 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: calc.engineer
provider_slug: calc-engineer
slug: calc-engineer-agentic-access
source_filename: calc-engineer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/calc-engineer-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 181\n  by_action_class:\n    connected: 91\n    acting: 90\n  by_consequence:\n    read: 91\n    write: 53\n    safety-critical: 13\n    physical: 24\n  human_in_the_loop_required: 13\noperations:\n- path: /api\n  method: get\n  operationId: getToolCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/docs\n  method: get\n  operationId: getOpenApiSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/keys\n  method: post\n  operationId: issueApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys/{prefix}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/fspl\n  method: get\n  operationId: get_fspl\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fspl\n  method: post\n  operationId: compute_fspl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/link_budget\n  method: get\n  operationId: get_link_budget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/link_budget\n  method: post\n  operationId: compute_link_budget\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dipole\n  method: get\n  operationId: get_dipole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dipole\n  method: post\n  operationId: compute_dipole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/microstrip\n  method: get\n  operationId: get_microstrip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/microstrip\n  method: post\n  operationId: compute_microstrip\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/dbm_convert\n  method: get\n  operationId: get_dbm_convert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dbm_convert\n  method: post\n  operationId: compute_dbm_convert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/noise_figure_cascade\n  method: get\n  operationId: get_noise_figure_cascade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/noise_figure_cascade\n  method: post\n  operationId: compute_noise_figure_cascade\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/vswr\n  method: get\n  operationId: get_vswr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/vswr\n  method: post\n  operationId: compute_vswr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/attenuator_pi\n\
  \  method: get\n  operationId: get_attenuator_pi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/attenuator_pi\n  method: post\n  operationId: compute_attenuator_pi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/attenuator_tee\n  method: get\n  operationId: get_attenuator_tee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/attenuator_tee\n  method: post\n  operationId: compute_attenuator_tee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fresnel_zone\n  method: get\n  operationId: get_fresnel_zone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fresnel_zone\n  method: post\n  operationId: compute_fresnel_zone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/wavelength_freq\n  method: get\n  operationId: get_wavelength_freq\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wavelength_freq\n  method: post\n  operationId:\
  \ compute_wavelength_freq\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/spice_template\n  method: get\n  operationId: get_spice_template\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/spice_template\n  method: post\n  operationId: compute_spice_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/spice_simulate\n  method: get\n  operationId:\
  \ get_spice_simulate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/spice_simulate\n  method: post\n  operationId: compute_spice_simulate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/lora_airtime\n  method: get\n  operationId: get_lora_airtime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lora_airtime\n  method: post\n  operationId: compute_lora_airtime\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/snr_margin\n  method: get\n  operationId: get_snr_margin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/snr_margin\n  method: post\n  operationId: compute_snr_margin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/channel_utilization\n  method: get\n  operationId: get_channel_utilization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/channel_utilization\n  method: post\n  operationId:\
  \ compute_channel_utilization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/lora_range_estimate\n  method: get\n  operationId: get_lora_range_estimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lora_range_estimate\n  method: post\n  operationId: compute_lora_range_estimate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/lora_sensitivity\n  method: get\n  operationId: get_lora_sensitivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lora_sensitivity\n  method: post\n  operationId: compute_lora_sensitivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/duty_cycle_budget\n  method: get\n  operationId: get_duty_cycle_budget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/duty_cycle_budget\n  method: post\n  operationId: compute_duty_cycle_budget\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/meshtastic_range\n  method: get\n  operationId: get_meshtastic_range\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meshtastic_range\n  method: post\n  operationId: compute_meshtastic_range\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/eirp_compliance\n  method: get\n  operationId: get_eirp_compliance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/eirp_compliance\n  method: post\n  operationId: compute_eirp_compliance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/meshtastic_power\n  method: get\n  operationId: get_meshtastic_power\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meshtastic_power\n  method: post\n  operationId: compute_meshtastic_power\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/lora_param_optimizer\n  method: get\n  operationId: get_lora_param_optimizer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lora_param_optimizer\n  method: post\n  operationId: compute_lora_param_optimizer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/zfs_capacity\n  method: get\n  operationId: get_zfs_capacity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/zfs_capacity\n  method: post\n  operationId: compute_zfs_capacity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/zfs_ram\n  method: get\n  operationId: get_zfs_ram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/zfs_ram\n  method: post\n  operationId: compute_zfs_ram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tcp_throughput\n  method: get\n  operationId: get_tcp_throughput\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tcp_throughput\n  method: post\n  operationId: compute_tcp_throughput\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/wireguard_mtu\n  method: get\n  operationId: get_wireguard_mtu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wireguard_mtu\n  method: post\n  operationId: compute_wireguard_mtu\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n   \
  \   exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/subnet_calculator\n  method: get\n  operationId: get_subnet_calculator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/subnet_calculator\n  method: post\n  operationId: compute_subnet_calculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/raid_iops\n  method: get\n  operationId: get_raid_iops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/raid_iops\n  method: post\n  operationId: compute_raid_iops\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/power_cost\n  method: get\n  operationId: get_power_cost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/power_cost\n  method: post\n  operationId: compute_power_cost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cooling_btu\n  method: get\n  operationId: get_cooling_btu\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cooling_btu\n  method: post\n  operationId: compute_cooling_btu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rack_capacity\n  method: get\n  operationId: get_rack_capacity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rack_capacity\n  method: post\n  operationId: compute_rack_capacity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/network_bandwidth\n  method: get\n  operationId: get_network_bandwidth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/network_bandwidth\n  method: post\n  operationId: compute_network_bandwidth\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/thermal_enclosure\n  method: get\n  operationId: get_thermal_enclosure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/thermal_enclosure\n  method: post\n  operationId:\
  \ compute_thermal_enclosure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/heatsink_cfd\n  method: get\n  operationId: get_heatsink_cfd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/heatsink_cfd\n  method: post\n  operationId: compute_heatsink_cfd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pcb_thermal\n  method: get\n  operationId: get_pcb_thermal\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pcb_thermal\n  method: post\n  operationId: compute_pcb_thermal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/battery_life\n  method: get\n  operationId: get_battery_life\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/battery_life\n  method: post\n  operationId: compute_battery_life\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/wire_gauge\n  method: get\n  operationId: get_wire_gauge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wire_gauge\n  method: post\n  operationId: compute_wire_gauge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/solar_sizing\n  method: get\n  operationId: get_solar_sizing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solar_sizing\n  method: post\n  operationId: compute_solar_sizing\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ups_runtime\n  method: get\n  operationId: get_ups_runtime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ups_runtime\n  method: post\n  operationId: compute_ups_runtime\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/mah_to_wh\n  method: get\n  operationId: get_mah_to_wh\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mah_to_wh\n  method: post\n  operationId: compute_mah_to_wh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/watts_to_amps\n  method: get\n  operationId: get_watts_to_amps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/watts_to_amps\n  method: post\n  operationId: compute_watts_to_amps\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/voltage_drop\n  method: get\n  operationId: get_voltage_drop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/voltage_drop\n  method: post\n  operationId: compute_voltage_drop\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/battery_charge_time\n  method: get\n  operationId: get_battery_charge_time\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/battery_charge_time\n\
  \  method: post\n  operationId: compute_battery_charge_time\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/solar_load_audit\n  method: get\n  operationId: get_solar_load_audit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solar_load_audit\n  method: post\n  operationId: compute_solar_load_audit\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /api/solar_roi\n  method: get\n  operationId: get_solar_roi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/solar_roi\n  method: post\n  operationId: compute_solar_roi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/battery_autonomy\n  method: get\n  operationId: get_battery_autonomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/battery_autonomy\n  method: post\n  operationId: compute_battery_autonomy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/string_sizing\n  method: get\n  operationId: get_string_sizing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/string_sizing\n  method: post\n  operationId: compute_string_sizing\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/generator_offset\n  method: get\n  operationId: get_generator_offset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/generator_offset\n  method: post\n  operationId: compute_generator_offset\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/wire_ampacity\n  method: get\n  operationId: get_wire_ampacity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/wire_ampacity\n  method: post\n  operationId: compute_wire_ampacity\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inverter_sizing\n  method: get\n  operationId: get_inverter_sizing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/inverter_sizing\n  method: post\n  operationId: compute_inverter_sizing\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/pcb_layout\n  method: get\n  operationId: get_pcb_layout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pcb_layout\n  method: post\n\
  \  operationId: compute_pcb_layout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/voltage_divider\n  method: get\n  operationId: get_voltage_divider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/voltage_divider\n  method: post\n  operationId: compute_voltage_divider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/rc_filter\n  method: get\n  operationId: get_rc_filter\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (51 KB total) ---\n# Full source: https://artifacts.apis.io/calc-engineer/agentic-access/calc-engineer-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/calc-engineer/agentic-access/calc-engineer-agentic-access.yml
summary_line: 181 operations · 90 acting · 13 human-in-the-loop
tags:
- Company
- Engineering
- Simulation
- Calculator
---
