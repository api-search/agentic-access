---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 48
api_specs:
- filename: africacompliancedata-com-countries-api-openapi.yml
  format: yaml
  label: africacompliancedata-com Countries API
  slug: africacompliancedata-com-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/africacompliancedata-com/openapi/africacompliancedata-com-countries-api-openapi.yml
- filename: africacompliancedata-com-holidays-and-business-days-api-openapi.yml
  format: yaml
  label: africacompliancedata-com Holidays and business days API
  slug: africacompliancedata-com-holidays-and-business-days-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/africacompliancedata-com/openapi/africacompliancedata-com-holidays-and-business-days-api-openapi.yml
- filename: africacompliancedata-com-private-mode-api-openapi.yml
  format: yaml
  label: africacompliancedata-com Private mode API
  slug: africacompliancedata-com-private-mode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/africacompliancedata-com/openapi/africacompliancedata-com-private-mode-api-openapi.yml
- filename: africacompliancedata-com-public-api-openapi.yml
  format: yaml
  label: africacompliancedata-com Public API
  slug: africacompliancedata-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/africacompliancedata-com/openapi/africacompliancedata-com-public-api-openapi.yml
- filename: africacompliancedata-com-tax-data-api-openapi.yml
  format: yaml
  label: africacompliancedata-com Tax data API
  slug: africacompliancedata-com-tax-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/africacompliancedata-com/openapi/africacompliancedata-com-tax-data-api-openapi.yml
- filename: africacompliancedata-com-webhooks-api-openapi.yml
  format: yaml
  label: africacompliancedata-com Webhooks API
  slug: africacompliancedata-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/africacompliancedata-com/openapi/africacompliancedata-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 48
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Africacompliancedata Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{id}/test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{id}/test
operation_count: 58
overview: 'africacompliancedata-com exposes 58 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 48 read, 8 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: africacompliancedata-com
provider_slug: africacompliancedata-com
slug: africacompliancedata-com-agentic-access
source_filename: africacompliancedata-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/africacompliancedata-com-openapi.json, openapi/africacompliancedata-com.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 58\n  by_action_class:\n    connected: 48\n    acting: 10\n  by_consequence:\n    read: 48\n    write: 8\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /calendar/{country}.ics\n  method: get\n  operationId: getPublicHolidayFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/account/countries\n  method: get\n  operationId: getCountryPack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/countries\n  method: post\n  operationId: setCountryPack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/changes\n  method: get\n  operationId: getChanges\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/holidays/watch\n  method: get\n  operationId: getHolidayWatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}\n  method: get\n  operationId: getCountryProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/holidays\n  method: get\n  operationId: getPublicHolidays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/countries/{country}/holidays.ics\n  method: get\n  operationId: getHolidayCalendarFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/is-business-day\n  method: get\n  operationId: isBusinessDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/business-days\n  method: get\n  operationId: countBusinessDays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/add-business-days\n  method: get\n  operationId: addBusinessDays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/countries/{country}/vat\n  method: get\n  operationId: getVat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/vat/history\n  method: get\n  operationId: getVatHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/withholding-tax\n  method: get\n  operationId: getWithholdingTax\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/treaties\n  method: get\n  operationId: getTaxTreaties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/finance-law\n  method: get\n  operationId:\
  \ getFinanceLaw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/payroll-tax\n  method: get\n  operationId: getPayrollTax\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/social-security\n  method: get\n  operationId: getSocialSecurity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/tax-id/validate\n  method: post\n  operationId: validateTaxIdFormatPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/countries/{country}/tax-id/validate\n  method: get\n  operationId: validateTaxIdFormat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tax-id/rules\n  method: get\n  operationId: getTaxIdRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/bundle\n  method: get\n  operationId: getCountryBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/deadlines\n  method: get\n  operationId: getFilingDeadlines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calendar/{country}.ics\n  method:\
  \ get\n  operationId: getPublicHolidayFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/countries\n  method: get\n  operationId: getCountryPack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/countries\n  method: post\n  operationId: setCountryPack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n\
  \  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/changes\n  method: get\n  operationId: getChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/holidays/watch\n  method: get\n  operationId: getHolidayWatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}\n  method: get\n  operationId:\
  \ getCountryProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/holidays\n  method: get\n  operationId: getPublicHolidays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/holidays.ics\n  method: get\n  operationId: getHolidayCalendarFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/is-business-day\n  method: get\n  operationId: isBusinessDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/business-days\n  method: get\n  operationId: countBusinessDays\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/add-business-days\n  method: get\n  operationId: addBusinessDays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/vat\n  method: get\n  operationId: getVat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/vat/history\n  method: get\n  operationId: getVatHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/withholding-tax\n  method: get\n  operationId: getWithholdingTax\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/treaties\n  method: get\n  operationId: getTaxTreaties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/finance-law\n  method: get\n  operationId: getFinanceLaw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/payroll-tax\n  method: get\n  operationId: getPayrollTax\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/social-security\n  method: get\n  operationId: getSocialSecurity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/countries/{country}/tax-id/validate\n  method: post\n  operationId: validateTaxIdFormatPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/countries/{country}/tax-id/validate\n  method: get\n  operationId: validateTaxIdFormat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tax-id/rules\n  method: get\n  operationId: getTaxIdRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/bundle\n  method: get\n  operationId: getCountryBundle\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries/{country}/deadlines\n  method: get\n  operationId: getFilingDeadlines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/africacompliancedata-com/agentic-access/africacompliancedata-com-agentic-access.yml
summary_line: 58 operations · 10 acting
tags:
- Africa
- Compliance
- Tax
- Holidays
- Data
---
