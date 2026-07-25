---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 22
api_specs:
- filename: red-hat-3scale-accounts-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Accounts API
  slug: red-hat-3scale-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-accounts-api-openapi.yml
- filename: red-hat-3scale-applications-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Applications API
  slug: red-hat-3scale-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-applications-api-openapi.yml
- filename: red-hat-3scale-authorization-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Authorization API
  slug: red-hat-3scale-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-authorization-api-openapi.yml
- filename: red-hat-3scale-configuration-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Configuration API
  slug: red-hat-3scale-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-configuration-api-openapi.yml
- filename: red-hat-3scale-dns-api-openapi.yml
  format: yaml
  label: Red Hat 3scale DNS API
  slug: red-hat-3scale-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-dns-api-openapi.yml
- filename: red-hat-3scale-health-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Health API
  slug: red-hat-3scale-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-health-api-openapi.yml
- filename: red-hat-3scale-initialization-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Initialization API
  slug: red-hat-3scale-initialization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-initialization-api-openapi.yml
- filename: red-hat-3scale-invoices-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Invoices API
  slug: red-hat-3scale-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-invoices-api-openapi.yml
- filename: red-hat-3scale-oauth-api-openapi.yml
  format: yaml
  label: Red Hat 3scale OAuth API
  slug: red-hat-3scale-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-oauth-api-openapi.yml
- filename: red-hat-3scale-payment-transactions-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Payment Transactions API
  slug: red-hat-3scale-payment-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-payment-transactions-api-openapi.yml
- filename: red-hat-3scale-plans-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Plans API
  slug: red-hat-3scale-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-plans-api-openapi.yml
- filename: red-hat-3scale-reporting-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Reporting API
  slug: red-hat-3scale-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-reporting-api-openapi.yml
- filename: red-hat-3scale-services-api-openapi.yml
  format: yaml
  label: Red Hat 3scale Services API
  slug: red-hat-3scale-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/openapi/red-hat-3scale-services-api-openapi.yml
consequence_counts:
  read: 22
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Red Hat 3Scale Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Red Hat 3scale exposes 32 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Red Hat 3scale
provider_slug: red-hat-3scale
slug: red-hat-3scale-agentic-access
source_filename: red-hat-3scale-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/red-hat-3scale-account-management-openapi.yml, openapi/red-hat-3scale-analytics-openapi.yml,\n  openapi/red-hat-3scale-apicast-management-openapi.yml, openapi/red-hat-3scale-billing-openapi.yml,\n  openapi/red-hat-3scale-service-management-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 22\n    acting: 10\n  by_consequence:\n    read: 22\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts.json\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts.json\n\
  \  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}.json\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}.json\n  method: put\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}.json\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/applications.json\n  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/applications.json\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}/applications/{id}.json\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/applications/{id}.json\n  method: put\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services.json\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{id}.json\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /application_plans.json\n  method: get\n  operationId: listApplicationPlans\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{service_id}/usage.json\n  method: get\n  operationId: getServiceUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}/usage.json\n  method: get\n  operationId: getApplicationUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{service_id}/top_applications.json\n  method: get\n  operationId: getTopApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n  operationId: getConfig\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: post\n  operationId: updateConfigPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config\n  method: put\n  operationId: updateConfigPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /config\n  method: delete\n  operationId: deleteConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /boot\n  method: post\n  operationId: bootGateway\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns/cache\n  method: get\n  operationId: getDnsCache\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/ready\n  method: get\n  operationId: getReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/live\n  method: get\n  operationId: getLiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/info\n  method: get\n  operationId: getStatusInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/invoices.json\n  method: get\n  operationId: listAccountInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}/invoices/{id}.json\n  method: get\n  operationId: getAccountInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices.json\n  method: get\n  operationId: listAllInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{id}/payment_transactions.json\n\
  \  method: get\n  operationId: listInvoicePaymentTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/authorize.xml\n  method: get\n  operationId: authorizeTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/authrep.xml\n  method: get\n  operationId: authorizeAndReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions.xml\n  method: post\n  operationId: reportTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /transactions/oauth_authorize.xml\n  method: get\n  operationId: oauthAuthorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-3scale/refs/heads/main/agentic-access/red-hat-3scale-agentic-access.yml
summary_line: 32 operations · 10 acting
tags:
- API Gateway
- API Management
- Developer Portal
- Enterprise
- Red Hat
---
