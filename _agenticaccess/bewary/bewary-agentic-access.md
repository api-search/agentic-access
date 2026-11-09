---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 29
api_specs:
- filename: bewary-account-api-openapi.yml
  format: yaml
  label: Bewary Account API
  slug: bewary-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-account-api-openapi.yml
- filename: bewary-app-api-openapi.yml
  format: yaml
  label: Bewary App API
  slug: bewary-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-app-api-openapi.yml
- filename: bewary-assess-api-openapi.yml
  format: yaml
  label: Bewary Assess API
  slug: bewary-assess-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-assess-api-openapi.yml
- filename: bewary-backtest-api-openapi.yml
  format: yaml
  label: Bewary Backtest API
  slug: bewary-backtest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-backtest-api-openapi.yml
- filename: bewary-batch-api-openapi.yml
  format: yaml
  label: Bewary Batch API
  slug: bewary-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-batch-api-openapi.yml
- filename: bewary-billing-api-openapi.yml
  format: yaml
  label: Bewary Billing API
  slug: bewary-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-billing-api-openapi.yml
- filename: bewary-bulk-api-openapi.yml
  format: yaml
  label: Bewary Bulk API
  slug: bewary-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-bulk-api-openapi.yml
- filename: bewary-calibration-api-openapi.yml
  format: yaml
  label: Bewary Calibration API
  slug: bewary-calibration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-calibration-api-openapi.yml
- filename: bewary-datasets-api-openapi.yml
  format: yaml
  label: Bewary Datasets API
  slug: bewary-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-datasets-api-openapi.yml
- filename: bewary-directory-api-openapi.yml
  format: yaml
  label: Bewary Directory API
  slug: bewary-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-directory-api-openapi.yml
- filename: bewary-domain-api-openapi.yml
  format: yaml
  label: Bewary Domain API
  slug: bewary-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-domain-api-openapi.yml
- filename: bewary-email-api-openapi.yml
  format: yaml
  label: Bewary Email API
  slug: bewary-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-email-api-openapi.yml
- filename: bewary-events-api-openapi.yml
  format: yaml
  label: Bewary Events API
  slug: bewary-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-events-api-openapi.yml
- filename: bewary-iban-api-openapi.yml
  format: yaml
  label: Bewary Iban API
  slug: bewary-iban-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-iban-api-openapi.yml
- filename: bewary-ip-api-openapi.yml
  format: yaml
  label: Bewary Ip API
  slug: bewary-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-ip-api-openapi.yml
- filename: bewary-keys-api-openapi.yml
  format: yaml
  label: Bewary Keys API
  slug: bewary-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-keys-api-openapi.yml
- filename: bewary-payment-handle-api-openapi.yml
  format: yaml
  label: Bewary Payment Handle API
  slug: bewary-payment-handle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-payment-handle-api-openapi.yml
- filename: bewary-phone-api-openapi.yml
  format: yaml
  label: Bewary Phone API
  slug: bewary-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-phone-api-openapi.yml
- filename: bewary-shortcode-api-openapi.yml
  format: yaml
  label: Bewary Shortcode API
  slug: bewary-shortcode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-shortcode-api-openapi.yml
- filename: bewary-url-api-openapi.yml
  format: yaml
  label: Bewary URL API
  slug: bewary-url-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-url-api-openapi.yml
- filename: bewary-wallet-api-openapi.yml
  format: yaml
  label: Bewary Wallet API
  slug: bewary-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-wallet-api-openapi.yml
- filename: bewary-watches-api-openapi.yml
  format: yaml
  label: Bewary Watches API
  slug: bewary-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-watches-api-openapi.yml
- filename: bewary-webhooks-api-openapi.yml
  format: yaml
  label: Bewary Webhooks API
  slug: bewary-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bewary/openapi/bewary-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 29
  safety-critical: 4
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Bewary Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/watches/{watch_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/webhooks/{webhook_id}/enable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/card
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
operation_count: 47
overview: 'Bewary exposes 47 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 12 write, 2 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bewary
provider_slug: bewary
slug: bewary-agentic-access
source_filename: bewary-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bewary-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 29\n    acting: 18\n  by_consequence:\n    read: 29\n    write: 12\n    safety-critical: 4\n    physical: 2\n  human_in_the_loop_required: 4\noperations:\n- path: /v1/domain/{host}\n  method: get\n  operationId: lookupDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domain/{host}/related\n  method: get\n  operationId: relatedDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /v1/url\n  method: get\n  operationId: lookupUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ip/{ip}\n  method: get\n  operationId: lookupIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/phone/{number}\n  method: get\n  operationId: lookupPhone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shortcode/{country}/{code}\n  method: get\n  operationId: lookupShortcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/email/{address}\n  method: get\n  operationId: lookupEmail\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallet/{chain}/{address}\n  method: get\n  operationId: lookupWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/iban/{iban}\n  method: get\n  operationId: lookupIban\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/{store}/{app_id}\n  method: get\n  operationId: lookupApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment-handle/{provider}/{handle}\n  method: get\n  operationId: lookupPaymentHandle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/batch\n  method: post\n  operationId: batchLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/assess\n  method: post\n  operationId: assessAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/{key_id}\n  method: patch\n  operationId: updateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/keys/{key_id}\n  method: delete\n  operationId: revokeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/checkout\n  method: post\n  operationId: startCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/portal\n  method: post\n  operationId: openBillingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/settings\n  method:\
  \ get\n  operationId: getBillingSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/settings\n  method: put\n  operationId: updateBillingSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/card\n  method: post\n  operationId: saveCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/card\n  method: delete\n  operationId:\
  \ dropCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watches\n  method: post\n  operationId: createWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watches\n  method: get\n  operationId: listWatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watches/{watch_id}\n  method: get\n  operationId: getWatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watches/{watch_id}\n  method: delete\n  operationId: deleteWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{webhook_id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhook_id}/rotate\n  method: post\n  operationId: rotateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhook_id}/enable\n  method: post\n  operationId: enableWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calibration/site\n  method: get\n  operationId: siteCalibration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/directory/area-codes\n  method: get\n  operationId: directoryAreaCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/directory/area-code/{npa}\n  method: get\n  operationId: directoryAreaCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/directory/number/{e164}\n  method: get\n  operationId: directoryNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/directory/numbers\n  method: get\n  operationId: directoryNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backtest\n  method: post\n  operationId: createBacktest\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/backtest/{backtest_id}\n  method: get\n  operationId: getBacktest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backtest/{backtest_id}\n  method: delete\n  operationId: deleteBacktest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bulk\n  method: get\n  operationId: bulkManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bulk/notices\n  method: get\n  operationId: bulkNotices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bulk/{fmt}\n  method: get\n  operationId: bulkFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bewary/agentic-access/bewary-agentic-access.yml
summary_line: 47 operations · 18 acting · 4 human-in-the-loop
tags:
- Company
- Security
- Fraud Prevention
- MCP
---
