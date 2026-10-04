---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 19
api_specs:
- filename: ibanforge-api-keys-api-openapi.yml
  format: yaml
  label: IBANforge API Keys API
  slug: ibanforge-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-api-keys-api-openapi.yml
- filename: ibanforge-bic-api-openapi.yml
  format: yaml
  label: IBANforge BIC API
  slug: ibanforge-bic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-bic-api-openapi.yml
- filename: ibanforge-compliance-api-openapi.yml
  format: yaml
  label: IBANforge Compliance API
  slug: ibanforge-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-compliance-api-openapi.yml
- filename: ibanforge-credits-api-openapi.yml
  format: yaml
  label: IBANforge Credits API
  slug: ibanforge-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-credits-api-openapi.yml
- filename: ibanforge-free-api-openapi.yml
  format: yaml
  label: IBANforge Free API
  slug: ibanforge-free-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-free-api-openapi.yml
- filename: ibanforge-iban-api-openapi.yml
  format: yaml
  label: IBANforge IBAN API
  slug: ibanforge-iban-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-iban-api-openapi.yml
- filename: ibanforge-mcp-api-openapi.yml
  format: yaml
  label: IBANforge MCP API
  slug: ibanforge-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-mcp-api-openapi.yml
- filename: ibanforge-swiss-clearing-api-openapi.yml
  format: yaml
  label: IBANforge Swiss Clearing API
  slug: ibanforge-swiss-clearing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-swiss-clearing-api-openapi.yml
- filename: ibanforge-account-api-openapi.yml
  format: yaml
  label: IBANforge Account API
  slug: ibanforge-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-account-api-openapi.yml
consequence_counts:
  physical: 2
  read: 19
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Ibanforge Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/keys/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/feedback
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/reference/validate
operation_count: 39
overview: 'IBANforge exposes 39 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 17 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IBANforge
provider_slug: ibanforge
slug: ibanforge-agentic-access
source_filename: ibanforge-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: generated\nsource: openapi/ibanforge-account-api-openapi.yml, openapi/ibanforge-api-keys-api-openapi.yml,\n  openapi/ibanforge-bic-api-openapi.yml, openapi/ibanforge-compliance-api-openapi.yml, openapi/ibanforge-credits-api-openapi.yml,\n  openapi/ibanforge-free-api-openapi.yml, openapi/ibanforge-iban-api-openapi.yml, openapi/ibanforge-mcp-api-openapi.yml,\n  openapi/ibanforge-swiss-clearing-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 20\n    connected: 19\n  by_consequence:\n    write: 17\n    read: 19\n    safety-critical: 1\n    physical: 2\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/account/code\n  method: post\n  operationId: requestAccountSignInCode\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/session\n  method: post\n  operationId: openAccountSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/overview\n  method: get\n  operationId: getAccountOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/keys/report\n  method: get\n  operationId: getAccountKeyReport\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/logout\n  method: post\n  operationId: closeAccountSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/generate\n  method: post\n  operationId: generateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/device\n  method: post\n  operationId: openDeviceGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/device/token\n  method: post\n  operationId: collectDeviceGrantKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/device/lookup\n  method: post\n  operationId: lookupDeviceGrant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/device/approve\n  method: post\n  operationId: approveDeviceGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/device/deny\n  method: post\n  operationId: denyDeviceGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/usage\n  method: get\n  operationId: getApiKeyUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/report\n  method: get\n  operationId: getApiKeyReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/revoke\n  method: post\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/keys/claim\n  method: post\n  operationId: claimApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/rotate\n  method: post\n  operationId: rotateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stats\n  method: get\n  operationId:\
  \ getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats/history\n  method: get\n  operationId: getStatsHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bic/{code}\n  method: get\n  operationId: lookupBIC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/iban/compliance\n  method: post\n  operationId: complianceCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credits/balance\n  method: get\n  operationId: getCreditBalance\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/bundles\n  method: get\n  operationId: listCreditBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/buy/{bundle}\n  method: post\n  operationId: buyCreditBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/iban/format\n  method: get\n  operationId: formatCheckIBAN\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ch/qr-bill/check\n  method: post\n  operationId:\
  \ checkSwissQrBill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/address/check\n  method: post\n  operationId: checkPostalAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reference/validate\n  method: get\n  operationId: validatePaymentReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reference/validate\n  method: post\n  operationId: validatePaymentReferencePost\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/iban/structure\n  method: get\n  operationId: listIBANStructures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/iban/structure/{country}\n  method: get\n  operationId: getIBANStructure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feedback\n  method: post\n  operationId: submitFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feedback/{id}\n  method: get\n  operationId: getFeedbackStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/test-iban\n  method: get\n  operationId: getTestIban\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/demo\n  method: get\n  operationId: getDemo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/iban/validate\n  method: post\n  operationId: validateIBAN\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/iban/batch\n  method: post\n  operationId: batchValidateIBAN\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcpStreamableHttp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/ch/clearing/{iid}\n  method: get\n  operationId: lookupChClearing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/agentic-access/ibanforge-agentic-access.yml
summary_line: 39 operations · 20 acting · 1 human-in-the-loop
tags:
- Finance
- Banking
- Compliance
- MCP
- A2A
---
