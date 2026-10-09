---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 47
api_specs:
- filename: travel-risk-api-adb-api-openapi.yml
  format: yaml
  label: Travel Risk API Adb API
  slug: travel-risk-api-adb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-adb-api-openapi.yml
- filename: travel-risk-api-auth-api-openapi.yml
  format: yaml
  label: Travel Risk API Auth API
  slug: travel-risk-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-auth-api-openapi.yml
- filename: travel-risk-api-billing-api-openapi.yml
  format: yaml
  label: Travel Risk API Billing API
  slug: travel-risk-api-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-billing-api-openapi.yml
- filename: travel-risk-api-ext-api-openapi.yml
  format: yaml
  label: Travel Risk API Ext API
  slug: travel-risk-api-ext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-ext-api-openapi.yml
- filename: travel-risk-api-public-data-api-openapi.yml
  format: yaml
  label: Travel Risk API Public Data API
  slug: travel-risk-api-public-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-public-data-api-openapi.yml
- filename: travel-risk-api-system-api-openapi.yml
  format: yaml
  label: Travel Risk API System API
  slug: travel-risk-api-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-system-api-openapi.yml
- filename: travel-risk-api-usage-api-openapi.yml
  format: yaml
  label: Travel Risk API Usage API
  slug: travel-risk-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/openapi/travel-risk-api-usage-api-openapi.yml
consequence_counts:
  physical: 3
  read: 47
  safety-critical: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Travel Risk Api Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/trips/{trip_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/billing/credits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/trips/{trip_id}/test-notification
operation_count: 61
overview: 'Travel Risk API exposes 61 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 47 read, 10 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Travel Risk API
provider_slug: travel-risk-api
slug: travel-risk-api-agentic-access
source_filename: travel-risk-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/travel-risk-api-aviation-openapi.yml, openapi/travel-risk-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 61\n  by_action_class:\n    connected: 47\n    acting: 14\n  by_consequence:\n    read: 47\n    write: 10\n    safety-critical: 1\n    physical: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /ext/v1/airport/{iata}/status\n  method: get\n  operationId: airport_status_ext_v1_airport__iata__status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/airport/{iata}/security\n  method: get\n  operationId: airport_security_ext_v1_airport__iata__security_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/airport/{iata}/immigration\n  method: get\n  operationId: airport_immigration_ext_v1_airport__iata__immigration_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/airport/{iata}/weather\n  method: get\n  operationId: airport_weather_ext_v1_airport__iata__weather_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/airport/{iata}/summary\n  method: get\n  operationId: airport_summary_ext_v1_airport__iata__summary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/border/{port}\n  method:\
  \ get\n  operationId: border_ext_v1_border__port__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/aircraft/{reg}\n  method: get\n  operationId: aircraft_by_reg_ext_v1_aircraft__reg__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/geoip/{ip}\n  method: get\n  operationId: geoip_lookup_ext_v1_geoip__ip__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/flights/coverage\n  method: get\n  operationId: flights_coverage_ext_v1_flights_coverage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/prices/history\n  method: get\n  operationId:\
  \ history_route_ext_v1_prices_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/prices/calendar\n  method: get\n  operationId: calendar_route_ext_v1_prices_calendar_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/prices/snapshots\n  method: post\n  operationId: prices_snapshots_202_ext_v1_prices_snapshots_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ext/v1/prices/watchlist\n  method: get\n  operationId: prices_watchlist_200_ext_v1_prices_watchlist_get\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/prices/watchlist\n  method: post\n  operationId: prices_watchlist_200_ext_v1_prices_watchlist_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ext/v1/prices/watchlist\n  method: delete\n  operationId: prices_watchlist_200_ext_v1_prices_watchlist_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ext/v1/prices/watchlist/{row_id}\n  method: delete\n  operationId: prices_watchlist_200_ext_v1_prices_watchlist__row_id__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ext/v1/airline/{iata}/profile\n  method: get\n  operationId: airline_profile_ext_v1_airline__iata__profile_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/airline/changes\n  method: get\n  operationId: airline_changes_ext_v1_airline_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/starlink/changes\n  method: get\n  operationId: starlink_changes_ext_v1_starlink_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/stats/usage\n  method: get\n  operationId: stats_usage_ext_v1_stats_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/stats/health\n  method: get\n  operationId: stats_health_ext_v1_stats_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/aircraft/{reg}/wifi\n  method: get\n  operationId: aircraft_wifi_ext_v1_aircraft__reg__wifi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/flight/{flight_iata}/wifi\n  method: get\n  operationId: flight_wifi_ext_v1_flight__flight_iata__wifi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/airline/{iata}/wifi\n  method: get\n  operationId: airline_wifi_ext_v1_airline__iata__wifi_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/starlink/fleet\n  method: get\n  operationId: starlink_fleet_ext_v1_starlink_fleet_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/v1/wifi/reports\n  method: post\n  operationId: submit_report_ext_v1_wifi_reports_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adb/airports/iata/{code}\n  method: get\n \
  \ operationId: adb_airports_iata_adb_airports_iata__code__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adb/airports/icao/{code}\n  method: get\n  operationId: adb_airports_icao_adb_airports_icao__code__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adb/airports/search/location\n  method: get\n  operationId: adb_airports_search_location_adb_airports_search_location_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adb/airports/search/ip\n  method: get\n  operationId: adb_airports_search_ip_adb_airports_search_ip_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /adb/aircrafts/Reg/{reg}\n  method: get\n  operationId: adb_aircrafts_reg_adb_aircrafts_Reg__reg__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adb/aircrafts/reg/{reg}\n  method: get\n  operationId: adb_aircrafts_reg_adb_aircrafts_reg__reg__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adb/aircrafts/icao24/{hex}\n  method: get\n  operationId: adb_aircrafts_icao24_adb_aircrafts_icao24__hex__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adb/airports/iata/{code}/weather\n  method: get\n  operationId: adb_airports_weather_adb_airports_iata__code__weather_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adb/airports/icao/{code}/weather\n  method: get\n  operationId: adb_airports_weather_adb_airports_icao__code__weather_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adb/airports/iata/{code}/weather/{from}/{to}\n  method: get\n  operationId: adb_airports_weather_range_adb_airports_iata__code__weather__from___to__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adb/flights/number/{number}\n  method: get\n  operationId: adb_flights_number_adb_flights_number__number__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adb/flights/number/{number}/{date}\n  method: get\n  operationId: adb_flights_number_date_adb_flights_number__number___date__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adb/flights/{number}/delays\n  method: get\n  operationId: adb_flights_delays_adb_flights__number__delays_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/health\n  method: get\n  operationId: health_check_api_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/countries/codes\n  method: get\n  operationId: list_country_codes_api_v1_countries_codes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/countries\n  method: get\n  operationId: get_countries_api_v1_countries_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/countries/{iso_code}\n  method: get\n  operationId: get_country_api_v1_countries__iso_code__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/alerts\n  method: get\n  operationId: get_alerts_api_v1_alerts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/alerts/{alert_id}\n  method: get\n  operationId: get_alert_api_v1_alerts__alert_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/risk-score/{iso_code}\n  method: get\n  operationId: get_risk_score_api_v1_risk_score__iso_code__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trips/assess\n  method: post\n  operationId: assess_trip_api_v1_trips_assess_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/trips\n  method: post\n  operationId: watch_trip_api_v1_trips_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/trips\n  method: get\n  operationId: list_trips_api_v1_trips_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trips/{trip_id}\n  method: get\n  operationId: get_trip_api_v1_trips__trip_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trips/{trip_id}\n  method: delete\n  operationId: stop_trip_api_v1_trips__trip_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/trips/{trip_id}/test-notification\n  method: post\n  operationId: test_trip_notification_api_v1_trips__trip_id__test_notification_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/conflicts\n  method: get\n  operationId: get_conflicts_api_v1_conflicts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/advisories\n  method: get\n  operationId: get_advisories_api_v1_advisories_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/plans\n  method: get\n  operationId: list_plans_api_v1_billing_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/checkout\n  method:\
  \ post\n  operationId: create_checkout_api_v1_billing_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/credits\n  method: post\n  operationId: buy_credits_api_v1_billing_credits_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/portal\n  method: post\n  operationId: billing_portal_api_v1_billing_portal_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/usage\n  method: get\n  operationId: get_usage_api_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/register\n  method: post\n  operationId: register_api_key_api_v1_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recover-key\n  method: post\n  operationId: recover_key_api_v1_recover_key_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travel-risk-api/refs/heads/main/agentic-access/travel-risk-api-agentic-access.yml
summary_line: 61 operations · 14 acting · 1 human-in-the-loop
tags:
- Travel
- Travel Risk
- Travel Advisories
- Aviation
- Airports
- Risk Scoring
- Safety
- Disaster Alerts
---
