---
acting_count: 123
action_class_counts:
  acting: 123
  connected: 1
api_specs:
- filename: calcfleet-com-ai-api-openapi.yml
  format: yaml
  label: CalcFleet AI API
  slug: calcfleet-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-ai-api-openapi.yml
- filename: calcfleet-com-auto-api-openapi.yml
  format: yaml
  label: CalcFleet Auto API
  slug: calcfleet-com-auto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-auto-api-openapi.yml
- filename: calcfleet-com-business-api-openapi.yml
  format: yaml
  label: CalcFleet Business API
  slug: calcfleet-com-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-business-api-openapi.yml
- filename: calcfleet-com-cooking-api-openapi.yml
  format: yaml
  label: CalcFleet Cooking API
  slug: calcfleet-com-cooking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-cooking-api-openapi.yml
- filename: calcfleet-com-debt-api-openapi.yml
  format: yaml
  label: CalcFleet Debt API
  slug: calcfleet-com-debt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-debt-api-openapi.yml
- filename: calcfleet-com-fitness-api-openapi.yml
  format: yaml
  label: CalcFleet Fitness API
  slug: calcfleet-com-fitness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-fitness-api-openapi.yml
- filename: calcfleet-com-freelance-api-openapi.yml
  format: yaml
  label: CalcFleet Freelance API
  slug: calcfleet-com-freelance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-freelance-api-openapi.yml
- filename: calcfleet-com-home-api-openapi.yml
  format: yaml
  label: CalcFleet Home API
  slug: calcfleet-com-home-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-home-api-openapi.yml
- filename: calcfleet-com-loans-api-openapi.yml
  format: yaml
  label: CalcFleet Loans API
  slug: calcfleet-com-loans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-loans-api-openapi.yml
- filename: calcfleet-com-mortgage-api-openapi.yml
  format: yaml
  label: CalcFleet Mortgage API
  slug: calcfleet-com-mortgage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-mortgage-api-openapi.yml
- filename: calcfleet-com-pet-api-openapi.yml
  format: yaml
  label: CalcFleet Pet API
  slug: calcfleet-com-pet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-pet-api-openapi.yml
- filename: calcfleet-com-photography-api-openapi.yml
  format: yaml
  label: CalcFleet Photography API
  slug: calcfleet-com-photography-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-photography-api-openapi.yml
- filename: calcfleet-com-pro-api-openapi.yml
  format: yaml
  label: CalcFleet Pro API
  slug: calcfleet-com-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-pro-api-openapi.yml
- filename: calcfleet-com-salary-api-openapi.yml
  format: yaml
  label: CalcFleet Salary API
  slug: calcfleet-com-salary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-salary-api-openapi.yml
- filename: calcfleet-com-savings-api-openapi.yml
  format: yaml
  label: CalcFleet Savings API
  slug: calcfleet-com-savings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-savings-api-openapi.yml
- filename: calcfleet-com-sport-api-openapi.yml
  format: yaml
  label: CalcFleet Sport API
  slug: calcfleet-com-sport-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calcfleet-com/openapi/calcfleet-com-sport-api-openapi.yml
consequence_counts:
  physical: 7
  read: 1
  write: 116
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Calcfleet Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tools/balance-transfer-calculator
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tools/car-lease-calculator
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tools/car-loan-calculator
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tools/down-payment-calculator
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tools/heloc-calculator
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tools/mortgage-overpayment-calculator
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tools/purchase-impact-calculator
operation_count: 124
overview: 'CalcFleet exposes 124 API operations that an AI agent could call, of which 123 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 116 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CalcFleet
provider_slug: calcfleet-com
slug: calcfleet-com-agentic-access
source_filename: calcfleet-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/calcfleet-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 124\n  by_action_class:\n    acting: 123\n    connected: 1\n  by_consequence:\n    physical: 7\n    write: 116\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/tools/mortgage-overpayment-calculator\n  method: post\n  operationId: mortgageOverpaymentCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/tools/debt-payoff-calculator\n  method: post\n  operationId: debtPayoffCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/freelance-hourly-rate-calculator\n  method: post\n  operationId: freelanceHourlyRateCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/compound-interest-calculator\n  method: post\n  operationId: compoundInterestCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/savings-goal-calculator\n  method: post\n  operationId: savingsGoalCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/car-loan-calculator\n  method: post\n  operationId: carLoanCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/break-even-calculator\n\
  \  method: post\n  operationId: breakEvenCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/margin-markup-calculator\n  method: post\n  operationId: marginMarkupCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/rent-vs-buy-calculator\n  method: post\n  operationId: rentVsBuyCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/fire-calculator\n  method: post\n  operationId: fireCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/take-home-pay-calculator\n  method: post\n  operationId: takeHomePayCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/student-loan-calculator\n  method: post\n  operationId: studentLoanCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/apy-calculator\n  method: post\n  operationId: apyCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/roi-calculator\n  method: post\n  operationId: roiCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/loan-amortization-calculator\n  method: post\n  operationId:\
  \ loanAmortizationCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/paint-calculator\n  method: post\n  operationId: paintCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/mortgage-refinance-calculator\n  method: post\n  operationId: mortgageRefinanceCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/tdee-calculator\n  method: post\n  operationId: tdeeCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/macro-calculator\n  method: post\n  operationId: macroCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/running-pace-calculator\n  method: post\n  operationId: runningPaceCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/rent-affordability-calculator\n  method: post\n  operationId: rentAffordabilityCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/closing-cost-calculator\n  method: post\n  operationId: closingCostCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/mortgage-points-calculator\n  method: post\n \
  \ operationId: mortgagePointsCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/home-affordability-calculator\n  method: post\n  operationId: homeAffordabilityCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/down-payment-calculator\n  method: post\n  operationId: downPaymentCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/mortgage-piti-calculator\n  method: post\n  operationId: mortgagePitiCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/balance-transfer-calculator\n  method: post\n  operationId: balanceTransferCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/heloc-calculator\n\
  \  method: post\n  operationId: helocCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/debt-consolidation-calculator\n  method: post\n  operationId: debtConsolidationCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/credit-card-payoff-calculator\n  method: post\n  operationId: creditCardPayoffCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/personal-loan-calculator\n  method: post\n  operationId: personalLoanCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/dti-calculator\n  method: post\n  operationId: dtiCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/saas-mrr-growth-calculator\n  method: post\n  operationId: saasMrrGrowthCalculator\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/cac-ltv-calculator\n  method: post\n  operationId: cacLtvCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/roas-calculator\n  method: post\n  operationId: roasCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/tools/churn-rate-calculator\n  method: post\n  operationId: churnRateCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/payback-period-calculator\n  method: post\n  operationId: paybackPeriodCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/burn-rate-runway-calculator\n  method: post\n  operationId: burnRateRunwayCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/product-pricing-calculator\n  method: post\n  operationId: productPricingCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/sales-tax-calculator\n  method: post\n  operationId: salesTaxCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/amazon-fba-calculator\n  method: post\n  operationId: amazonFbaCalculator\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/etsy-fee-calculator\n  method: post\n  operationId: etsyFeeCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/ecommerce-profit-margin-calculator\n  method: post\n  operationId: ecommerceProfitMarginCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/tools/solar-panel-savings-calculator\n  method: post\n  operationId: solarPanelSavingsCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/solar-system-size-calculator\n  method: post\n  operationId: solarSystemSizeCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/electricity-cost-calculator\n  method: post\n  operationId: electricityCostCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/ev-charging-cost-calculator\n  method: post\n  operationId: evChargingCostCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/heat-pump-savings-calculator\n  method: post\n  operationId: heatPumpSavingsCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/home-battery-size-calculator\n\
  \  method: post\n  operationId: homeBatterySizeCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/car-affordability-calculator\n  method: post\n  operationId: carAffordabilityCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/car-lease-calculator\n  method: post\n  operationId: carLeaseCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/lease-vs-buy-car-calculator\n  method: post\n  operationId: leaseVsBuyCarCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/car-depreciation-calculator\n  method: post\n  operationId: carDepreciationCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/cost-per-mile-calculator\n  method: post\n  operationId: costPerMileCalculator\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/gas-vs-electric-car-calculator\n  method: post\n  operationId: gasVsElectricCarCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/flooring-calculator\n  method: post\n  operationId: flooringCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /api/v1/tools/tile-calculator\n  method: post\n  operationId: tileCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/concrete-calculator\n  method: post\n  operationId: concreteCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/drywall-calculator\n  method: post\n  operationId: drywallCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/deck-boards-calculator\n  method: post\n  operationId: deckBoardsCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/fence-calculator\n  method: post\n  operationId: fenceCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/llm-api-cost-calculator\n  method: post\n  operationId: llmApiCostCalculator\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/token-counter-calculator\n  method: post\n  operationId: tokenCounterCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/ai-build-vs-buy-calculator\n  method: post\n  operationId: aiBuildVsBuyCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /api/v1/tools/gpu-vram-calculator\n  method: post\n  operationId: gpuVramCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/ai-roi-calculator\n  method: post\n  operationId: aiRoiCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/ai-job-exposure-calculator\n  method: post\n  operationId: aiJobExposureCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/salary-to-hourly-calculator\n  method: post\n  operationId: salaryToHourlyCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/overtime-pay-calculator\n  method: post\n  operationId: overtimePayCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/pay-raise-calculator\n  method: post\n  operationId: payRaiseCalculator\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/pto-accrual-calculator\n  method: post\n  operationId: ptoAccrualCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/contractor-vs-employee-calculator\n  method: post\n  operationId: contractorVsEmployeeCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/tools/employee-cost-calculator\n  method: post\n  operationId: employeeCostCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/401k-match-calculator\n  method: post\n  operationId: 401kMatchCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/roth-ira-calculator\n  method: post\n  operationId: rothIraCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/cd-ladder-calculator\n  method: post\n  operationId: cdLadderCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/coast-fire-calculator\n  method: post\n  operationId: coastFireCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/dividend-reinvestment-calculator\n  method: post\n  operationId: dividendReinvestmentCalculator\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/savings-drawdown-calculator\n  method: post\n  operationId: savingsDrawdownCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/retirement-monte-carlo-calculator\n  method: post\n  operationId: retirementMonteCarloCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/mulch-calculator\n  method: post\n  operationId: mulchCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/topsoil-calculator\n  method: post\n  operationId: topsoilCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/grass-seed-calculator\n  method: post\n  operationId: grassSeedCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/gravel-calculator\n  method: post\n  operationId: gravelCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/fertilizer-calculator\n  method: post\n  operationId: fertilizerCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/one-rep-max-calculator\n  method: post\n  operationId: oneRepMaxCalculator\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/body-fat-calculator\n  method: post\n  operationId: bodyFatCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/ideal-weight-calculator\n  method: post\n  operationId: idealWeightCalculator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n\n\n# --- truncated at 32 KB (44 KB total) ---\n# Full source: https://artifacts.apis.io/calcfleet-com/agentic-access/calcfleet-com-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/calcfleet-com/agentic-access/calcfleet-com-agentic-access.yml
summary_line: 124 operations · 123 acting
tags:
- Calculator
- Artificial Intelligence
- VCC
- Free
---
