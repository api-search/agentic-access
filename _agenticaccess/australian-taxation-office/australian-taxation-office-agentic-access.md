---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 12
api_specs:
- filename: australian-taxation-office-apiinfo-api-openapi.yml
  format: yaml
  label: Australian Taxation Office API Info API
  slug: australian-taxation-office-apiinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-apiinfo-api-openapi.yml
- filename: australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Combined Global and Domestic Group Entity Tax Return API
  slug: australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-combined-global-and-domestic-group-entity-tax-return-api-openapi.yml
- filename: australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Combined Global and Domestic Minimum Tax Return API
  slug: australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-combined-global-and-domestic-minimum-tax-return-api-openapi.yml
- filename: australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Get Payee Stapled Super Fund for Receipt API
  slug: australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-get-payee-stapled-super-fund-for-receipt-api-openapi.yml
- filename: australian-taxation-office-get-payment-reference-number-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Get Payment Reference Number API
  slug: australian-taxation-office-get-payment-reference-number-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-get-payment-reference-number-api-openapi.yml
- filename: australian-taxation-office-gst-property-settlement-date-confirmation-api-openapi.yml
  format: yaml
  label: Australian Taxation Office GST Property Settlement Date Confirmation API
  slug: australian-taxation-office-gst-property-settlement-date-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-gst-property-settlement-date-confirmation-api-openapi.yml
- filename: australian-taxation-office-gst-property-settlement-withholding-notification-api-openapi.yml
  format: yaml
  label: Australian Taxation Office GST Property Settlement Withholding Notification API
  slug: australian-taxation-office-gst-property-settlement-withholding-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-gst-property-settlement-withholding-notification-api-openapi.yml
- filename: australian-taxation-office-heartbeat-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Heartbeat API
  slug: australian-taxation-office-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-heartbeat-api-openapi.yml
- filename: australian-taxation-office-providers-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Providers API
  slug: australian-taxation-office-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-providers-api-openapi.yml
- filename: australian-taxation-office-register-a-new-software-application-instance-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Register a new software application instance API
  slug: australian-taxation-office-register-a-new-software-application-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-register-a-new-software-application-instance-api-openapi.yml
- filename: australian-taxation-office-request-stapled-super-fund-for-payee-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Request Stapled Super Fund for Payee API
  slug: australian-taxation-office-request-stapled-super-fund-for-payee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-request-stapled-super-fund-for-payee-api-openapi.yml
- filename: australian-taxation-office-spec-api-openapi.yml
  format: yaml
  label: Australian Taxation Office Spec API
  slug: australian-taxation-office-spec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/openapi/australian-taxation-office-spec-api-openapi.yml
consequence_counts:
  read: 12
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Australian Taxation Office Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Australian Taxation Office exposes 20 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Australian Taxation Office
provider_slug: australian-taxation-office
slug: australian-taxation-office-agentic-access
source_filename: australian-taxation-office-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: generated\nsource: openapi/australian-taxation-office-global-domestic-minimum-group-entity-tax-return-openapi.yml,\n  openapi/australian-taxation-office-global-domestic-minimum-tax-return-openapi.yml, openapi/australian-taxation-office-gst-property-settlement-openapi.yml,\n  openapi/australian-taxation-office-health-check-openapi.yml, openapi/australian-taxation-office-oauth-dynamic-client-registration-openapi.yml,\n  openapi/australian-taxation-office-payment-reference-number-openapi.yml, openapi/australian-taxation-office-smsf-alias-lookup-openapi.yml,\n  openapi/australian-taxation-office-stapled-super-fund-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 8\n\
  \    connected: 12\n  by_consequence:\n    write: 8\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /clients/ABN/{identifierValue}/globalDomesticReturn/{transactionID}/groupEntity\n  method: post\n  operationId: requestGlobalDomesticGroupEntityTaxReturnForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clients/ABN/{identifierValue}/globalDomesticReturn\n  method: post\n  operationId: requestGlobalDomesticMinimumTaxReturnFormABN\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clients/ABN/{identifierValue}/propertySettlements\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - ato.apGSTPropertySettlement\n- path: /clients/ABN/{identifierValue}/propertySettlements/validationResults\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - ato.apGSTPropertySettlement\n- path: /clients/ABN/{identifierValue}/changeOfPropertySettlements\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - ato.apGSTPropertySettlement\n- path: /clients/ABN/{identifierValue}/changeOfPropertySettlements/validationResults\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - ato.apGSTPropertySettlement\n- path: /heartbeat\n  method: get\n  operationId: GetHeartbeat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ato.healthcheck.*.*\n- path: /clients/ABN/{abn_business}/individuals/TFN/{tfn_individual}/heartbeat\n  method: get\n  operationId: GetHeartbeatABN\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ato.healthcheck.*.*\n- path: /clients/WPN/{wpn_business}/individuals/TFN/{tfn_individual}/heartbeat\n  method: get\n  operationId: GetHeartbeatWPN\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ato.healthcheck.*.*\n- path: /\n  method: get\n  operationId: GetStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ato.healthcheck.*.*\n- path: /specs/yaml\n  method: get\n  operationId: GetSpecYaml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ato.healthcheck.*.*\n- path: /specs/spec.yaml\n  method: get\n  operationId:\
  \ DownloadSpecYaml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ato.healthcheck.*.*\n- path: /\n  method: post\n  operationId: postClientRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: retrievePaymentReferenceNumberFormat4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers\n  method: get\n  operationId: GetProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method:\
  \ get\n  operationId: GetStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /specs/yaml\n  method: get\n  operationId: GetSpecYaml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /specs/spec.yaml\n  method: get\n  operationId: DownloadSpecYaml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: requestStapledSuperFundForPayeeWithAbn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - ato.super.stapledsuperfund.c,r\n\
  - path: /{receipt}\n  method: get\n  operationId: requestStapledSuperFundForPayeeWithReceiptNumberAndAbn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - ato.super.stapledsuperfund.c,r\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-taxation-office/refs/heads/main/agentic-access/australian-taxation-office-agentic-access.yml
summary_line: 20 operations · 8 acting
tags:
- Company
- Government
- Taxation
- Superannuation
- Australia
- Digital Service Providers
- Public Sector
---
