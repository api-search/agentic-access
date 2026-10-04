---
acting_count: 35
action_class_counts:
  acting: 35
  connected: 28
api_specs:
- filename: starlink-telemetry-asyncapi.yml
  format: yaml
  label: Starlink Telemetry Stream API
  slug: starlink-telemetry-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/asyncapi/starlink-telemetry-asyncapi.yml
- filename: starlink-account-api-openapi.yml
  format: yaml
  label: Starlink Account API
  slug: starlink-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-account-api-openapi.yml
- filename: starlink-addresses-api-openapi.yml
  format: yaml
  label: Starlink Addresses API
  slug: starlink-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-addresses-api-openapi.yml
- filename: starlink-billing-api-openapi.yml
  format: yaml
  label: Starlink Billing API
  slug: starlink-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-billing-api-openapi.yml
- filename: starlink-contacts-api-openapi.yml
  format: yaml
  label: Starlink Contacts API
  slug: starlink-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-contacts-api-openapi.yml
- filename: starlink-data-pools-api-openapi.yml
  format: yaml
  label: Starlink Data Pools API
  slug: starlink-data-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-data-pools-api-openapi.yml
- filename: starlink-flights-api-openapi.yml
  format: yaml
  label: Starlink Flights API
  slug: starlink-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-flights-api-openapi.yml
- filename: starlink-managed-accounts-api-openapi.yml
  format: yaml
  label: Starlink Managed Accounts API
  slug: starlink-managed-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-managed-accounts-api-openapi.yml
- filename: starlink-managed-api-openapi.yml
  format: yaml
  label: Starlink Managed API
  slug: starlink-managed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-managed-api-openapi.yml
- filename: starlink-mobile-api-openapi.yml
  format: yaml
  label: Starlink Mobile API
  slug: starlink-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-mobile-api-openapi.yml
- filename: starlink-routers-api-openapi.yml
  format: yaml
  label: Starlink Routers API
  slug: starlink-routers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-routers-api-openapi.yml
- filename: starlink-service-lines-api-openapi.yml
  format: yaml
  label: Starlink Service Lines API
  slug: starlink-service-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-service-lines-api-openapi.yml
- filename: starlink-user-terminals-api-openapi.yml
  format: yaml
  label: Starlink User Terminals API
  slug: starlink-user-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-user-terminals-api-openapi.yml
consequence_counts:
  read: 28
  safety-critical: 3
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Starlink Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v2/data-pools/{dataPoolId}/set-automatic-top-up
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v2/routers/{routerId}/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /public/v2/user-terminals/{deviceId}/reboot
operation_count: 63
overview: 'Starlink exposes 63 API operations that an AI agent could call, of which 35 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 32 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Starlink
provider_slug: starlink
slug: starlink-agentic-access
source_filename: starlink-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/starlink-account-api-openapi.yml, openapi/starlink-addresses-api-openapi.yml,\n  openapi/starlink-billing-api-openapi.yml, openapi/starlink-contacts-api-openapi.yml, openapi/starlink-data-pools-api-openapi.yml,\n  openapi/starlink-flights-api-openapi.yml, openapi/starlink-managed-accounts-api-openapi.yml,\n  openapi/starlink-managed-api-openapi.yml, openapi/starlink-mobile-api-openapi.yml, openapi/starlink-routers-api-openapi.yml,\n  openapi/starlink-service-lines-api-openapi.yml, openapi/starlink-user-terminals-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 63\n  by_action_class:\n    connected: 28\n    acting: 35\n  by_consequence:\n    read: 28\n    write: 32\n \
  \   safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /public/v2/account\n  method: get\n  operationId: getPublicV2Account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/data-usage/query\n  method: post\n  operationId: postPublicV2DataUsageQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/products\n  method: get\n  operationId: getPublicV2Products\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/addresses\n  method: get\n  operationId: getPublicV2Addresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/addresses\n\
  \  method: post\n  operationId: postPublicV2Addresses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/addresses/{addressReferenceId}\n  method: get\n  operationId: getPublicV2AddressesByAddressReferenceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/addresses/{addressReferenceId}\n  method: put\n  operationId: putPublicV2AddressesByAddressReferenceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /public/v2/billing/invoices\n  method: get\n  operationId: getPublicV2BillingInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/billing/invoices/{invoiceId}\n  method: get\n  operationId: getPublicV2BillingInvoicesByInvoiceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/billing/balance\n  method: get\n  operationId: getPublicV2BillingBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/contacts\n  method: get\n  operationId: getPublicV2Contacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/contacts\n\
  \  method: post\n  operationId: postPublicV2Contacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/contacts/{subjectId}\n  method: delete\n  operationId: deletePublicV2ContactsBySubjectId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/contacts/{subjectId}\n  method: put\n  operationId: putPublicV2ContactsBySubjectId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/data-pools\n  method: get\n  operationId: getPublicV2DataPools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/data-pools/usage\n  method: get\n  operationId: getPublicV2DataPoolsUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/data-pools/{dataPoolId}/set-automatic-top-up\n  method: post\n  operationId: postPublicV2DataPoolsByDataPoolIdSetAutomaticTopUp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /public/v2/flights/status\n  method: post\n  operationId: postPublicV2FlightsStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/managed/accounts/tree\n  method: get\n  operationId: getPublicV2ManagedAccountsTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/managed/accounts\n  method: get\n  operationId: getPublicV2ManagedAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/managed/customers\n  method: post\n  operationId: postPublicV2ManagedCustomers\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/mobile/radio-access-network/{timestamp}\n  method: get\n  operationId: getPublicV2MobileRadioAccessNetworkByTimestamp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/mobile/timeseries/{timestamp}\n  method: get\n  operationId: getPublicV2MobileTimeseriesByTimestamp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/mobile/map/{timestamp}\n  method: get\n  operationId: getPublicV2MobileMapByTimestamp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/routers/{routerId}\n  method: get\n  operationId: getPublicV2RoutersByRouterId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/routers/configs\n  method: get\n  operationId: getPublicV2RoutersConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/routers/configs\n  method: post\n  operationId: postPublicV2RoutersConfigs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/routers/configs/{configId}\n  method: get\n  operationId: getPublicV2RoutersConfigsByConfigId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/routers/configs/{configId}\n  method: put\n  operationId: putPublicV2RoutersConfigsByConfigId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/routers/configs/assign\n  method: put\n  operationId: putPublicV2RoutersConfigsAssign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/routers/configs/default\n  method: get\n  operationId: getPublicV2RoutersConfigsDefault\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/routers/configs/default\n  method: put\n  operationId: putPublicV2RoutersConfigsDefault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/routers/configs/tls\n  method: get\n  operationId: getPublicV2RoutersConfigsTls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/routers/configs/tls\n  method: post\n  operationId: postPublicV2RoutersConfigsTls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/routers/configs/tls\n  method: delete\n  operationId: deletePublicV2RoutersConfigsTls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/routers/local-content\n  method: post\n  operationId: postPublicV2RoutersLocalContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/routers/local-content\n  method: get\n  operationId: getPublicV2RoutersLocalContent\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/routers/sandbox/clients\n  method: get\n  operationId: getPublicV2RoutersSandboxClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/routers/sandbox/clients\n  method: post\n  operationId: postPublicV2RoutersSandboxClients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/routers/sandbox/heartbeat\n  method: put\n  operationId: putPublicV2RoutersSandboxHeartbeat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/routers/{routerId}/reboot\n  method: post\n  operationId: postPublicV2RoutersByRouterIdReboot\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v2/service-lines/{serviceLineNumber}\n  method: get\n  operationId: getPublicV2ServiceLinesByServiceLineNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/service-lines/{serviceLineNumber}\n  method: delete\n  operationId: deletePublicV2ServiceLinesByServiceLineNumber\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/service-lines\n  method: get\n  operationId: getPublicV2ServiceLines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/service-lines\n  method: post\n  operationId: postPublicV2ServiceLines\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/service-lines/{serviceLineNumber}/nickname\n  method: put\n  operationId: putPublicV2ServiceLinesByServiceLineNumberNickname\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/service-lines/{serviceLineNumber}/product\n  method: put\n  operationId: putPublicV2ServiceLinesByServiceLineNumberProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/service-lines/{serviceLineNumber}/public-ip\n  method: put\n  operationId: putPublicV2ServiceLinesByServiceLineNumberPublicIp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/service-lines/{serviceLineNumber}/data/opt-in\n  method: post\n  operationId: postPublicV2ServiceLinesByServiceLineNumberDataOptIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/service-lines/{serviceLineNumber}/data/opt-out\n  method: post\n  operationId: postPublicV2ServiceLinesByServiceLineNumberDataOptOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/service-lines/{serviceLineNumber}/user-terminals\n\
  \  method: post\n  operationId: postPublicV2ServiceLinesByServiceLineNumberUserTerminals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/service-lines/{serviceLineNumber}/user-terminals/{deviceId}\n  method: delete\n  operationId: deletePublicV2ServiceLinesByServiceLineNumberUserTerminalsByDeviceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/service-lines/{serviceLineNumber}/data/recurring\n  method: put\n  operationId: putPublicV2ServiceLinesByServiceLineNumberDataRecurring\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/service-lines/{serviceLineNumber}/data/top-up\n  method: post\n  operationId: postPublicV2ServiceLinesByServiceLineNumberDataTopUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/service-lines/{serviceLineNumber}/billing-cycles/partial-periods\n  method: get\n  operationId: getPublicV2ServiceLinesByServiceLineNumberBillingCyclesPartialPeriods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /public/v2/service-lines/{serviceLineNumber}/consume-from-pool\n  method: patch\n  operationId: patchPublicV2ServiceLinesByServiceLineNumberConsumeFromPool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/user-terminals\n  method: get\n  operationId: getPublicV2UserTerminals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/user-terminals\n  method: post\n  operationId: postPublicV2UserTerminals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/user-terminals/{deviceId}\n  method: delete\n  operationId: deletePublicV2UserTerminalsByDeviceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/user-terminals/{deviceId}/reboot\n  method: post\n  operationId: postPublicV2UserTerminalsByDeviceIdReboot\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/v2/user-terminals/configs/assign\n  method: put\n  operationId: putPublicV2UserTerminalsConfigsAssign\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v2/user-terminals/l2vpn\n  method: get\n  operationId: getPublicV2UserTerminalsL2vpn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v2/user-terminals/{deviceId}/l2vpn\n  method: put\n  operationId: putPublicV2UserTerminalsByDeviceIdL2vpn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/agentic-access/starlink-agentic-access.yml
summary_line: 63 operations · 35 acting · 3 human-in-the-loop
tags:
- Non-Terrestrial Network
- Starlink
- Telecommunications
- United States
- Satellite
- Broadband
- Connectivity
- Device Management
- Telemetry
- Aviation
- Maritime
- Enterprise
---
