---
acting_count: 79
action_class_counts:
  acting: 79
  connected: 54
api_specs:
- filename: metronome-alerts-api-openapi.yml
  format: yaml
  label: Metronome Alerts API
  slug: metronome-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-alerts-api-openapi.yml
- filename: metronome-billable-metrics-api-openapi.yml
  format: yaml
  label: Metronome Billable Metrics API
  slug: metronome-billable-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-billable-metrics-api-openapi.yml
- filename: metronome-contracts-api-openapi.yml
  format: yaml
  label: Metronome Contracts API
  slug: metronome-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-contracts-api-openapi.yml
- filename: metronome-credits-and-commits-api-openapi.yml
  format: yaml
  label: Metronome Credits and commits API
  slug: metronome-credits-and-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-credits-and-commits-api-openapi.yml
- filename: metronome-custom-fields-api-openapi.yml
  format: yaml
  label: Metronome Custom fields API
  slug: metronome-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-custom-fields-api-openapi.yml
- filename: metronome-customers-api-openapi.yml
  format: yaml
  label: Metronome Customers API
  slug: metronome-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-customers-api-openapi.yml
- filename: metronome-integrations-api-openapi.yml
  format: yaml
  label: Metronome Integrations API
  slug: metronome-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-integrations-api-openapi.yml
- filename: metronome-invoices-api-openapi.yml
  format: yaml
  label: Metronome Invoices API
  slug: metronome-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-invoices-api-openapi.yml
- filename: metronome-named-schedules-api-openapi.yml
  format: yaml
  label: Metronome Named schedules API
  slug: metronome-named-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-named-schedules-api-openapi.yml
- filename: metronome-notifications-api-openapi.yml
  format: yaml
  label: Metronome Notifications API
  slug: metronome-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-notifications-api-openapi.yml
- filename: metronome-packages-api-openapi.yml
  format: yaml
  label: Metronome Packages API
  slug: metronome-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-packages-api-openapi.yml
- filename: metronome-payments-api-openapi.yml
  format: yaml
  label: Metronome Payments API
  slug: metronome-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-payments-api-openapi.yml
- filename: metronome-products-api-openapi.yml
  format: yaml
  label: Metronome Products API
  slug: metronome-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-products-api-openapi.yml
- filename: metronome-rate-cards-api-openapi.yml
  format: yaml
  label: Metronome Rate cards API
  slug: metronome-rate-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-rate-cards-api-openapi.yml
- filename: metronome-security-api-openapi.yml
  format: yaml
  label: Metronome Security API
  slug: metronome-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-security-api-openapi.yml
- filename: metronome-settings-api-openapi.yml
  format: yaml
  label: Metronome Settings API
  slug: metronome-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-settings-api-openapi.yml
- filename: metronome-threshold-billing-api-openapi.yml
  format: yaml
  label: Metronome Threshold billing API
  slug: metronome-threshold-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-threshold-billing-api-openapi.yml
- filename: metronome-usage-api-openapi.yml
  format: yaml
  label: Metronome Usage API
  slug: metronome-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-usage-api-openapi.yml
consequence_counts:
  physical: 14
  read: 54
  safety-critical: 3
  write: 62
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Metronome Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/contracts/commits/disableTrueup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/customFields/removeKey
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/customer-alerts/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/composite/createCustomerWithContract
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/contract-pricing/rate-cards/moveRateCardProducts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/contract-pricing/rate-cards/setRateCardProductsOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/contracts/commits/threshold-billing/release
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/contracts/createHistoricalInvoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/contracts/scheduleProServicesInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/contracts/updateInvoiceIssueDate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/customers/{customer_id}/invoices/invoice_seats
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/customers/{customer_id}/previewEvents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoices/regenerate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoices/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/attempt
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/threshold-billing/update-active-recharge-config
operation_count: 133
overview: 'Metronome exposes 133 API operations that an AI agent could call, of which 79 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 54 read, 62 write, 14 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Metronome
provider_slug: metronome
slug: metronome-agentic-access
source_filename: metronome-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/metronome-alerts-api-openapi.yml, openapi/metronome-billable-metrics-api-openapi.yml,\n  openapi/metronome-contracts-api-openapi.yml, openapi/metronome-credits-and-commits-api-openapi.yml,\n  openapi/metronome-custom-fields-api-openapi.yml, openapi/metronome-customers-api-openapi.yml,\n  openapi/metronome-integrations-api-openapi.yml, openapi/metronome-invoices-api-openapi.yml,\n  openapi/metronome-named-schedules-api-openapi.yml, openapi/metronome-notifications-api-openapi.yml,\n  openapi/metronome-packages-api-openapi.yml, openapi/metronome-payments-api-openapi.yml, openapi/metronome-products-api-openapi.yml,\n  openapi/metronome-rate-cards-api-openapi.yml, openapi/metronome-security-api-openapi.yml,\n  openapi/metronome-settings-api-openapi.yml, openapi/metronome-threshold-billing-api-openapi.yml,\n  openapi/metronome-usage-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified\
  \ heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 133\n  by_action_class:\n    acting: 79\n    connected: 54\n  by_consequence:\n    write: 62\n    read: 54\n    safety-critical: 3\n    physical: 14\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/alerts/archive\n  method: post\n  operationId: archiveAlert-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alerts/create\n  method: post\n  operationId: createAlert-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer-alerts/get\n  method: post\n  operationId: getCustomerAlert-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer-alerts/list\n  method: post\n  operationId: listCustomerAlerts-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer-alerts/reset\n  method: post\n  operationId: resetCustomerAlerts-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/billable-metrics\n\
  \  method: post\n  operationId: createBillableMetric-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billable-metrics\n  method: get\n  operationId: listAllBillableMetrics-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billable-metrics/create\n  method: post\n  operationId: createBillableMetricV1-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billable-metrics/archive\n  method: post\n  operationId:\
  \ archiveBillableMetric-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billable-metrics/{billable_metric_id}\n  method: get\n  operationId: getBillableMetric-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billable-metrics/{billable_metric_id}\n  method: put\n  operationId: updateBillableMetric-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}/billable-metrics\n  method:\
  \ get\n  operationId: listBillableMetrics-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/get\n  method: post\n  operationId: getContract-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/list\n  method: post\n  operationId: listContracts-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/create\n  method: post\n  operationId: createContract-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/contracts/amend\n  method: post\n  operationId: amendContract-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/archive\n  method: post\n  operationId: archiveContract-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/setUsageFilter\n  method: post\n  operationId: setUsageFilter-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/updateInvoiceIssueDate\n  method: post\n  operationId: updateInvoiceIssueDate-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/updateEndDate\n  method: post\n  operationId: updateContractEndDate-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/getContractRateSchedule\n  method: post\n  operationId: getContractRateSchedule-v1\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/getSubscriptionQuantityHistory\n  method: post\n  operationId: getSubscriptionQuantityHistory-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/getSubscriptionSeatsHistory\n  method: post\n  operationId: getSubscriptionSeatsHistory-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/scheduleProServicesInvoice\n  method: post\n  operationId: scheduleProServicesInvoice-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/createHistoricalInvoices\n  method: post\n  operationId: createHistoricalContractUsageInvoices-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/composite/createCustomerWithContract\n  method: post\n  operationId: createCustomerWithContract-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/packages/create\n\
  \  method: post\n  operationId: createPackage-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/packages/listContractsOnPackage\n  method: post\n  operationId: listContractsOnPackage-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/contracts/get\n  method: post\n  operationId: getContract-v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/contracts/getEditHistory\n  method: post\n  operationId: getContractEditHistory-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/contracts/list\n  method: post\n  operationId: listContracts-v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/contracts/edit\n  method: post\n  operationId: editContract-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/addManualBalanceLedgerEntry\n  method: post\n  operationId: addManualBalanceLedgerEntry-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/customerCommits/list\n  method: post\n  operationId: listCustomerCommits-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/customerCommits/create\n  method: post\n  operationId: createCustomerCommit-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/customerCommits/updateEndDate\n  method: post\n  operationId: updateCommitEndDate-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/commits/threshold-billing/release\n  method: post\n  operationId: releaseExternalPaymentGateThresholdCommit-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/commits/disableTrueup\n  method: post\n  operationId: disableCommitTrueup-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v1/contracts/customerCredits/list\n  method: post\n  operationId: listCustomerCredits-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/customerCredits/create\n  method: post\n  operationId: createCustomerCredit-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/customerCredits/updateEndDate\n  method: post\n  operationId: updateCreditEndDate-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/contracts/customerBalances/list\n  method: post\n  operationId: listCustomerBalances-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/customerBalances/getNetBalance\n  method: post\n  operationId: getNetBalance-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/seatBalances/list\n  method: post\n  operationId: listSeatBalances-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/contracts/commits/edit\n  method: post\n  operationId: editCommit-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/contracts/credits/edit\n  method: post\n  operationId: editCredit-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/contracts/commits/archive\n  method: post\n  operationId: archiveCommit-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/contracts/credits/archive\n  method: post\n  operationId: archiveCredit-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customFields/addKey\n  method: post\n  operationId: addCustomFieldKey-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customFields/removeKey\n  method: post\n  operationId: disableCustomFieldKey-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/customFields/setValues\n\
  \  method: post\n  operationId: setCustomFields-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customFields/deleteValues\n  method: post\n  operationId: deleteCustomFields-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customFields/listKeys\n  method: post\n  operationId: listCustomFieldKeys-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/setBillableStatus\n  method: post\n  operationId:\
  \ setCustomerBillableStatus-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/archive\n  method: post\n  operationId: archiveCustomer-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}\n  method: get\n  operationId: getCustomer-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers\n  method: get\n  operationId: listCustomers-v1\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers\n  method: post\n  operationId: createCustomer-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}/setIngestAliases\n  method: post\n  operationId: setIngestAliases-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}/setName\n  method: post\n  operationId: setCustomerName-v1\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}/updateConfig\n  method: post\n  operationId: updateCustomerConfig-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/getCustomerBillingProviderConfigurations\n  method: post\n  operationId: getCustomerBillingProviderConfigurations-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/getCustomerRevenueSystemConfigurations\n  method: post\n  operationId: getCustomerRevenueSystemConfigurations-v1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/setCustomerBillingProviderConfigurations\n  method: post\n  operationId: setCustomerBillingProviderConfigurations-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/archiveCustomerBillingProviderConfigurations\n  method: post\n  operationId: archiveCustomerBillingProviderConfigurations-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/setCustomerRevenueSystemConfigurations\n\
  \  method: post\n  operationId: setCustomerRevenueSystemConfigurations-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/archiveCustomerRevenueSystemConfigurations\n  method: post\n  operationId: archiveCustomerRevenueSystemConfigurations-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dashboards/getEmbeddableUrl\n  method: post\n  operationId: embeddableDashboard-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/integrations/log\n  method: post\n  operationId: integrationCloudwatchLogger-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}/invoices/invoice_seats\n  method: post\n  operationId: chargeSeats-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}/invoices\n  method: get\n  operationId: listInvoices-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}/invoices/breakdowns\n  method: get\n  operationId: listBreakdownInvoices-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}/invoices/{invoice_id}/pdf\n  method: get\n  operationId: getInvoicePdf-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}/invoices/{invoice_id}\n  method: get\n  operationId: getInvoice-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}/invoices/spend-breakdowns\n  method: post\n  operationId: listSpendBreakdownInvoices-v1\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices/void\n  method: post\n  operationId: voidInvoice-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invoices/regenerate\n  method: post\n  operationId: regenerateInvoice-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}/previewEvents\n  method: post\n  operationId: previewCustomerEvents-v1\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/getNamedSchedule\n  method: post\n  operationId: getCustomerNamedSchedule-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/updateNamedSchedule\n  method: post\n  operationId: updateCustomerNamedSchedule-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contracts/getNamedSchedule\n\
  \  method: post\n  operationId: getContractNamedSchedule-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/listNamedSchedules\n  method: post\n  operationId: listContractsNamedSchedules-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contracts/updateNamedSchedule\n  method: post\n  operationId: updateContractNamedSchedule-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contract-pricing/rate-cards/getNamedSchedule\n  method: post\n  operationId: getRateCardNamedSchedule-v1\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contract-pricing/rate-cards/updateNamedSchedule\n  method: post\n  operationId: updateRateCardNamedSchedule-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/notifications/create\n  method: post\n  operationId: createNotificationConfig-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/notifications/get\n  method: post\n  operationId: getNotificationConfig-v2\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/notifications/offset/list\n  method: post\n  operationId: listOffsetNotificationConfigs-v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/notifications/system/list\n  method: post\n  operationId: listSystemNotificationConfigs-v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/notifications/edit\n  method: post\n  operationId: editNotificationConfig-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/notifications/archive\n\
  \  method: post\n  operationId: archiveNotificationConfig-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/packages/get\n  method: post\n  operationId: getPackage-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/packages/list\n  method: post\n  operationId: listPackages-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/packages/archive\n  method: post\n  operationId: archivePackage-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/attempt\n  method: post\n  operationId: attemptPayment-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/cancel\n  method: post\n  operationId: cancelPayment-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/list\n  method: post\n  operationId:\
  \ listPayments-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contract-pricing/products/get\n  method: post\n  operationId: getProduct-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contract-pricing/products/list\n  method: post\n  operationId: listProducts-v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contract-pricing/products/create\n  method: post\n  operationId: createProduct-v1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n\n\n# --- truncated at 32 KB (42 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/agentic-access/metronome-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/agentic-access/metronome-agentic-access.yml
summary_line: 133 operations · 79 acting · 3 human-in-the-loop
tags:
- Billing
- FinOps
- Metering
- Pricing
- Usage-Based Billing
---
