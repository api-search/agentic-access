---
acting_count: 46
action_class_counts:
  acting: 46
  connected: 6
api_specs:
- filename: calculate-co-nz-calculators-api-openapi.yml
  format: yaml
  label: Calculate.co.nz Calculators API
  slug: calculate-co-nz-calculators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculate-co-nz/openapi/calculate-co-nz-calculators-api-openapi.yml
- filename: calculate-co-nz-discovery-api-openapi.yml
  format: yaml
  label: Calculate.co.nz Discovery API
  slug: calculate-co-nz-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculate-co-nz/openapi/calculate-co-nz-discovery-api-openapi.yml
- filename: calculate-co-nz-reference-data-api-openapi.yml
  format: yaml
  label: Calculate.co.nz Reference data API
  slug: calculate-co-nz-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculate-co-nz/openapi/calculate-co-nz-reference-data-api-openapi.yml
- filename: calculate-co-nz-service-api-openapi.yml
  format: yaml
  label: Calculate.co.nz Service API
  slug: calculate-co-nz-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calculate-co-nz/openapi/calculate-co-nz-service-api-openapi.yml
consequence_counts:
  physical: 10
  read: 6
  write: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Calculate Co Nz Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/bonus-tax
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/citizenship-presence
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/import-duty
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/mortgage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/parental-leave
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/rates-water
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/road-user-charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/schedular-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/tax-refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/vehicle-loan
operation_count: 52
overview: 'Calculate.co.nz exposes 52 API operations that an AI agent could call, of which 46 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 36 write, and 10 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Calculate.co.nz
provider_slug: calculate-co-nz
slug: calculate-co-nz-agentic-access
source_filename: calculate-co-nz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/calculate-co-nz-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 6\n    acting: 46\n  by_consequence:\n    read: 6\n    write: 36\n    physical: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/index-status\n  method:\
  \ get\n  operationId: index_health_v1_index_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/find-calculator\n  method: post\n  operationId: find_calculator_v1_find_calculator_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/paye\n  method: post\n  operationId: paye_v1_paye_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gst\n  method: post\n  operationId: gst_v1_gst_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bmi\n  method: post\n  operationId: bmi_v1_bmi_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mortgage\n  method: post\n  operationId: mortgage_v1_mortgage_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/annual-leave\n  method: post\n  operationId: annual_leave_v1_annual_leave_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fuel-cost\n  method: post\n  operationId: fuel_cost_v1_fuel_cost_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tax-refund\n  method: post\n  operationId: tax_refund_v1_tax_refund_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /v1/gpa\n  method: post\n  operationId: gpa_v1_gpa_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hourly-to-salary\n  method: post\n  operationId: hourly_to_salary_v1_hourly_to_salary_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/work-hours\n  method: post\n  operationId: work_hours_v1_work_hours_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bonus-tax\n  method: post\n  operationId: bonus_tax_v1_bonus_tax_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/power-tower\n  method: post\n  operationId: power_tower_v1_power_tower_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parental-leave\n  method: post\n  operationId: parental_leave_v1_parental_leave_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/net-to-gross\n  method: post\n  operationId: net_to_gross_v1_net_to_gross_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/final-pay\n  method: post\n  operationId: final_pay_v1_final_pay_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/secondary-tax\n  method: post\n  operationId: secondary_tax_v1_secondary_tax_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pro-rata-salary\n  method: post\n  operationId: pro_rata_salary_v1_pro_rata_salary_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lump-sum-tax\n  method: post\n  operationId: lump_sum_tax_v1_lump_sum_tax_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/working-for-families\n  method: post\n  operationId: working_for_families_v1_working_for_families_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/road-user-charges\n  method: post\n  operationId: road_user_charges_v1_road_user_charges_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/electricity-cost\n  method: post\n  operationId: electricity_cost_v1_electricity_cost_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ncea-rank-score\n  method: post\n  operationId: ncea_rank_score_v1_ncea_rank_score_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vehicle-loan\n  method: post\n  operationId: vehicle_loan_v1_vehicle_loan_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n     \
  \ exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/energy-expenditure\n  method: post\n  operationId: energy_expenditure_v1_energy_expenditure_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rates\n  method: get\n  operationId: rates_v1_rates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rates/{rate_id}\n  method: get\n  operationId: rate_by_id_v1_rates__rate_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/kiwisaver\n  method: post\n  operationId: kiwisaver_v1_kiwisaver_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fbt\n  method: post\n  operationId: fbt_v1_fbt_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/redundancy-entitlement\n  method: post\n  operationId: redundancy_entitlement_v1_redundancy_entitlement_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/grocery-budget\n  method: post\n  operationId: grocery_budget_v1_grocery_budget_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contractor-vs-employee\n  method: post\n  operationId: contractor_vs_employee_v1_contractor_vs_employee_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/benefit-entitlement\n  method: post\n  operationId: benefit_entitlement_v1_benefit_entitlement_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schedular-payments\n  method: post\n  operationId: schedular_payments_v1_schedular_payments_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/acc-weekly-compensation\n  method: post\n  operationId: acc_weekly_compensation_v1_acc_weekly_compensation_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sick-leave\n  method: post\n  operationId: sick_leave_v1_sick_leave_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tax-code\n  method: post\n  operationId: tax_code_v1_tax_code_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/paye-due-dates\n  method: post\n  operationId: paye_due_dates_v1_paye_due_dates_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/depreciation\n  method: post\n  operationId: depreciation_v1_depreciation_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/minimum-wage\n  method: post\n  operationId: minimum_wage_v1_minimum_wage_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/overtime-pay\n  method: post\n  operationId:\
  \ overtime_pay_v1_overtime_pay_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/citizenship-presence\n  method: post\n  operationId: citizenship_presence_v1_citizenship_presence_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/standard-drinks\n  method: post\n  operationId: standard_drinks_v1_standard_drinks_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ncea-grade\n  method: post\n  operationId: ncea_grade_v1_ncea_grade_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-holidays\n  method: post\n  operationId: public_holidays_v1_public_holidays_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/business-days\n  method: post\n  operationId: business_days_v1_business_days_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/holiday-pay\n  method: post\n  operationId: holiday_pay_v1_holiday_pay_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rates-water\n  method: post\n  operationId: rates_water_v1_rates_water_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/import-duty\n  method: post\n  operationId: import_duty_v1_import_duty_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/calculate-co-nz/agentic-access/calculate-co-nz-agentic-access.yml
summary_line: 52 operations · 46 acting
tags:
- Company
- Finance
- Calculators
- New Zealand
- Free
- Education
---
