---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 45
api_specs:
- filename: engrate-audit-logs-api-openapi.yml
  format: yaml
  label: Engrate Audit Logs API
  slug: engrate-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-audit-logs-api-openapi.yml
- filename: engrate-benachrichtigung-api-openapi.yml
  format: yaml
  label: Engrate Benachrichtigung API
  slug: engrate-benachrichtigung-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-benachrichtigung-api-openapi.yml
- filename: engrate-betrieb-api-openapi.yml
  format: yaml
  label: Engrate Betrieb API
  slug: engrate-betrieb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-betrieb-api-openapi.yml
- filename: engrate-clearing-api-openapi.yml
  format: yaml
  label: Engrate Clearing API
  slug: engrate-clearing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-clearing-api-openapi.yml
- filename: engrate-core-api-openapi.yml
  format: yaml
  label: Engrate Core API
  slug: engrate-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-core-api-openapi.yml
- filename: engrate-cost-of-energy-api-openapi.yml
  format: yaml
  label: Engrate Cost Of Energy API
  slug: engrate-cost-of-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-cost-of-energy-api-openapi.yml
- filename: engrate-geo-api-openapi.yml
  format: yaml
  label: Engrate Geo API
  slug: engrate-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-geo-api-openapi.yml
- filename: engrate-holidays-api-openapi.yml
  format: yaml
  label: Engrate Holidays API
  slug: engrate-holidays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-holidays-api-openapi.yml
- filename: engrate-lokationen-api-openapi.yml
  format: yaml
  label: Engrate Lokationen API
  slug: engrate-lokationen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-lokationen-api-openapi.yml
- filename: engrate-lokationsb-ndel-api-openapi.yml
  format: yaml
  label: Engrate Lokationsbündel API
  slug: engrate-lokationsb-ndel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-lokationsb-ndel-api-openapi.yml
- filename: engrate-mabis-api-openapi.yml
  format: yaml
  label: Engrate Mabis API
  slug: engrate-mabis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-mabis-api-openapi.yml
- filename: engrate-netzbetreiberwechsel-api-openapi.yml
  format: yaml
  label: Engrate Netzbetreiberwechsel API
  slug: engrate-netzbetreiberwechsel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-netzbetreiberwechsel-api-openapi.yml
- filename: engrate-nl-settlement-api-openapi.yml
  format: yaml
  label: Engrate Nl Settlement API
  slug: engrate-nl-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-nl-settlement-api-openapi.yml
- filename: engrate-profiles-api-openapi.yml
  format: yaml
  label: Engrate Profiles API
  slug: engrate-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-profiles-api-openapi.yml
- filename: engrate-reference-api-openapi.yml
  format: yaml
  label: Engrate Reference API
  slug: engrate-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-reference-api-openapi.yml
- filename: engrate-schedules-api-openapi.yml
  format: yaml
  label: Engrate Schedules API
  slug: engrate-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-schedules-api-openapi.yml
- filename: engrate-status-request-api-openapi.yml
  format: yaml
  label: Engrate Status Request API
  slug: engrate-status-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-status-request-api-openapi.yml
- filename: engrate-time-series-api-openapi.yml
  format: yaml
  label: Engrate Time Series API
  slug: engrate-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/openapi/engrate-time-series-api-openapi.yml
consequence_counts:
  physical: 2
  read: 45
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Engrate Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /schedule-management/v1/mabis/send-response-to-aggregation-time-series
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /schedule-management/v1/send_status_request
operation_count: 54
overview: 'Engrate exposes 54 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read, 7 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Engrate
provider_slug: engrate
slug: engrate-agentic-access
source_filename: engrate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: generated\nsource: openapi/engrate-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    connected: 45\n    acting: 9\n  by_consequence:\n    read: 45\n    write: 7\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /core/v1/bidding-zones\n  method: get\n  operationId: list_bidding_zones_core_v1_bidding_zones_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/control-areas\n  method: get\n  operationId: list_control_areas_core_v1_control_areas_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/geo\n  method: get\n  operationId: get_geodata_core_v1_geo_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/holidays\n  method: get\n  operationId: list_holidays_core_v1_holidays_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/metering-grid-areas\n  method: get\n  operationId: list_metering_grid_areas_core_v1_metering_grid_areas_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/parties\n  method: get\n  operationId: list_parties_core_v1_parties_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /core/v1/scheduling-areas\n  method: get\n  operationId: list_scheduling_areas_core_v1_scheduling_areas_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost-of-energy/v1/calculate\n  method: post\n  operationId: calculate_tariff_cost_of_energy_v1_calculate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cost-of-energy/v1/datasets\n  method: get\n  operationId: list_datasets_cost_of_energy_v1_datasets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost-of-energy/v1/profiles\n  method: get\n  operationId:\
  \ list_profiles_cost_of_energy_v1_profiles_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost-of-energy/v1/profiles\n  method: post\n  operationId: create_profile_cost_of_energy_v1_profiles_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cost-of-energy/v1/profiles/{profile_id}\n  method: delete\n  operationId: delete_profile_cost_of_energy_v1_profiles__profile_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /cost-of-energy/v1/profiles/{profile_id}\n  method: get\n  operationId: get_profile_cost_of_energy_v1_profiles__profile_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost-of-energy/v1/profiles/{profile_id}\n  method: put\n  operationId: update_profile_cost_of_energy_v1_profiles__profile_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cost-of-energy/v1/tariffs\n  method: get\n  operationId: list_tariffs_cost_of_energy_v1_tariffs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost-of-energy/v1/tariffs/{tariff_id}\n\
  \  method: get\n  operationId: get_tariff_cost_of_energy_v1_tariffs__tariff_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost-of-energy/v1/tariffs/{tariff_id}/simplified\n  method: get\n  operationId: get_simplified_tariff_cost_of_energy_v1_tariffs__tariff_id__simplified_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market-access/v1alpha1/timeseries/aggregate-allocations\n  method: get\n  operationId: list_aggregate_allocations_market_access_v1alpha1_timeseries_aggregate_allocations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market-access/v1alpha1/timeseries/allocations\n  method: get\n  operationId: list_allocations_market_access_v1alpha1_timeseries_allocations_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market-access/v1alpha1/timeseries/series/aggregate-allocations\n  method: get\n  operationId: list_aggregate_allocation_series_market_access_v1alpha1_timeseries_series_aggregate_allocations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/anomalies\n  method: get\n  operationId: list_anomalies_schedule_management_v1_anomalies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/audit-logs\n  method: get\n  operationId: list_audit_logs_schedule_management_v1_audit_logs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/aggregation-objects\n  method: get\n  operationId: list_aggregation_objects_schedule_management_v1_mabis_aggregation_objects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/clearing-calendar\n  method: get\n  operationId: get_clearing_calendar_schedule_management_v1_mabis_clearing_calendar_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/clearing-periods\n  method: get\n  operationId: list_clearing_periods_schedule_management_v1_mabis_clearing_periods_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/clearing-periods\n\
  \  method: post\n  operationId: create_clearing_period_schedule_management_v1_mabis_clearing_periods_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule-management/v1/mabis/clearing-periods/{uid}\n  method: get\n  operationId: get_clearing_period_schedule_management_v1_mabis_clearing_periods__uid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/clearing-periods/{uid}/imbalance\n  method: get\n  operationId: calculate_imbalance_schedule_management_v1_mabis_clearing_periods__uid__imbalance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/clearing-periods/{uid}/messages\n  method: get\n  operationId: list_messages_schedule_management_v1_mabis_clearing_periods__uid__messages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/clearing-periods/{uid}/objections\n  method: get\n  operationId: list_objections_schedule_management_v1_mabis_clearing_periods__uid__objections_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/clearing-periods/{uid}/objections\n  method: post\n  operationId: create_objection_schedule_management_v1_mabis_clearing_periods__uid__objections_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule-management/v1/mabis/clearing-periods/{uid}/settlements\n  method: get\n  operationId: list_settlements_schedule_management_v1_mabis_clearing_periods__uid__settlements_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/clearing-periods/{uid}/validate\n  method: get\n  operationId: validate_clearing_data_schedule_management_v1_mabis_clearing_periods__uid__validate_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/control-energy-prices\n  method: get\n  operationId: get_control_energy_prices_schedule_management_v1_mabis_control_energy_prices_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/energy-volumes\n  method: get\n  operationId: list_energy_volumes_schedule_management_v1_mabis_energy_volumes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/energy-volumes/{mabis_zp_id}/monthly-summary\n  method: get\n  operationId: get_monthly_summary_schedule_management_v1_mabis_energy_volumes__mabis_zp_id__monthly_summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/mabis/send-response-to-aggregation-time-series\n  method: post\n  operationId: send_response_to_aggregation_time_series_schedule_management_v1_mabis_send_response_to_aggregation_time_series_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule-management/v1/nl/settlement/imbalance-reports\n  method: get\n  operationId: list_imbalance_reports_schedule_management_v1_nl_settlement_imbalance_reports_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/nl/settlement/imbalance-reports/{uid}\n  method: get\n  operationId: get_imbalance_report_schedule_management_v1_nl_settlement_imbalance_reports__uid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/nl/settlement/imbalance-reports/{uid}/time-series\n\
  \  method: get\n  operationId: list_report_time_series_schedule_management_v1_nl_settlement_imbalance_reports__uid__time_series_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/nl/settlement/summary\n  method: get\n  operationId: get_summary_schedule_management_v1_nl_settlement_summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/reference/exchange-priority-balance-groups\n  method: get\n  operationId: list_exchange_priority_balance_groups_schedule_management_v1_reference_exchange_priority_balance_groups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/reference/exchange-priority-check/{eic_code}\n\
  \  method: get\n  operationId: check_exchange_priority_schedule_management_v1_reference_exchange_priority_check__eic_code__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/schedule-series/{version_uid}\n  method: get\n  operationId: get_schedule_series_schedule_management_v1_schedule_series__version_uid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/schedules\n  method: get\n  operationId: list_schedules_schedule_management_v1_schedules_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/schedules\n  method: post\n  operationId: create_schedule_schedule_management_v1_schedules_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule-management/v1/schedules/{uid}\n  method: get\n  operationId: get_schedule_schedule_management_v1_schedules__uid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/schedules/{uid}/anomalies\n  method: get\n  operationId: get_schedule_anomalies_schedule_management_v1_schedules__uid__anomalies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/schedules/{uid}/delivery-status\n  method: get\n  operationId: get_delivery_status_schedule_management_v1_schedules__uid__delivery_status_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/schedules/{uid}/incoming-messages\n  method: get\n  operationId: list_incoming_messages_schedule_management_v1_schedules__uid__incoming_messages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/schedules/{uid}/reconciliation\n  method: get\n  operationId: get_schedule_reconciliation_schedule_management_v1_schedules__uid__reconciliation_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/schedules/{uid}/versions\n  method: get\n  operationId: list_schedule_versions_schedule_management_v1_schedules__uid__versions_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/schedules/{uid}/versions/{version_number}\n  method: get\n  operationId: get_schedule_version_schedule_management_v1_schedules__uid__versions__version_number__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule-management/v1/send_status_request\n  method: post\n  operationId: send_status_request_schedule_management_v1_send_status_request_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engrate/refs/heads/main/agentic-access/engrate-agentic-access.yml
summary_line: 54 operations · 9 acting
tags:
- Company
- Energy
- Platform
- Integration
- Market
---
