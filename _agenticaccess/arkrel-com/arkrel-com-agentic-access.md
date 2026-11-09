---
acting_count: 51
action_class_counts:
  acting: 51
  connected: 37
api_specs:
- filename: arkrel-com-account-data-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Account Data API
  slug: arkrel-com-account-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-account-data-api-openapi.yml
- filename: arkrel-com-auth-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Auth API
  slug: arkrel-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-auth-api-openapi.yml
- filename: arkrel-com-billing-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Billing API
  slug: arkrel-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-billing-api-openapi.yml
- filename: arkrel-com-businesses-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Businesses API
  slug: arkrel-com-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-businesses-api-openapi.yml
- filename: arkrel-com-category-rules-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Category Rules API
  slug: arkrel-com-category-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-category-rules-api-openapi.yml
- filename: arkrel-com-chart-of-accounts-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Chart Of Accounts API
  slug: arkrel-com-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-chart-of-accounts-api-openapi.yml
- filename: arkrel-com-connections-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Connections API
  slug: arkrel-com-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-connections-api-openapi.yml
- filename: arkrel-com-documents-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Documents API
  slug: arkrel-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-documents-api-openapi.yml
- filename: arkrel-com-mcp-api-openapi.yml
  format: yaml
  label: Conecta Media LLC MCP API
  slug: arkrel-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-mcp-api-openapi.yml
- filename: arkrel-com-ops-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Ops API
  slug: arkrel-com-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-ops-api-openapi.yml
- filename: arkrel-com-schemas-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Schemas API
  slug: arkrel-com-schemas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-schemas-api-openapi.yml
- filename: arkrel-com-settings-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Settings API
  slug: arkrel-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-settings-api-openapi.yml
- filename: arkrel-com-statement-sets-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Statement Sets API
  slug: arkrel-com-statement-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-statement-sets-api-openapi.yml
- filename: arkrel-com-tax-report-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Tax Report API
  slug: arkrel-com-tax-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-tax-report-api-openapi.yml
- filename: arkrel-com-tax-years-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Tax Years API
  slug: arkrel-com-tax-years-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-tax-years-api-openapi.yml
- filename: arkrel-com-usage-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Usage API
  slug: arkrel-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-usage-api-openapi.yml
- filename: arkrel-com-webhooks-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Webhooks API
  slug: arkrel-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-webhooks-api-openapi.yml
- filename: arkrel-com-year-overview-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Year Overview API
  slug: arkrel-com-year-overview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-year-overview-api-openapi.yml
consequence_counts:
  physical: 7
  read: 37
  safety-critical: 2
  write: 42
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Arkrel Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/documents/{id}/categorization/undo
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/statement-sets/{id}/categorization/rows/{documentId}/{rowIndex}/undo
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /app/api/auth/step-up/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /app/api/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /app/api/billing/checkout-pack
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /app/api/billing/refund-autopilot
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/chart-of-accounts/settings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/documents/{id}/categorization
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/documents/{id}/categorize
operation_count: 88
overview: 'Conecta Media LLC exposes 88 API operations that an AI agent could call, of which 51 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 42 write, 7 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Conecta Media LLC
provider_slug: arkrel-com
slug: arkrel-com-agentic-access
source_filename: arkrel-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/arkrel-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 88\n  by_action_class:\n    connected: 37\n    acting: 51\n  by_consequence:\n    read: 37\n    write: 42\n    physical: 7\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /app/api/orgs\n  method: get\n  operationId: listBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/api/orgs\n  method: post\n  operationId: createBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/orgs/active\n  method: post\n  operationId: switchActiveBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/orgs/current\n  method: get\n  operationId: getCurrentBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/api/orgs/current\n  method: patch\n  operationId: updateCurrentBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/orgs/current\n  method: delete\n  operationId: deleteBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/orgs/current/leave\n  method: post\n  operationId: leaveBusiness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/data-export\n  method: get\n  operationId: listAccountDataExports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /app/api/data-export\n  method: post\n  operationId: createAccountDataExports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/data-export/{id}/download\n  method: get\n  operationId: downloadAccountDataExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal/maintenance/reencrypt\n  method: post\n  operationId: reencryptStoredSecrets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /app/api/plaid/connections\n  method: get\n  operationId: listBankConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/api/plaid/link-token\n  method: post\n  operationId: createBankLinkToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/plaid/exchange\n  method: post\n  operationId: exchangeBankPublicToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/plaid/connections/{id}/refresh\n\
  \  method: post\n  operationId: refreshBankConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/plaid/connections/{id}\n  method: delete\n  operationId: disconnectBankConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/plaid/webhook\n  method: post\n  operationId: receivePlaidWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ops/health\n  method: get\n  operationId: getOpsHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/api/settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/api/settings/notifications\n  method: patch\n  operationId: updateProcessingEmails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/auth/step-up\n  method: get\n  operationId: getStepUpMethods\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/api/auth/step-up\n  method: post\n  operationId: verifyStepUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/auth/step-up/email\n  method: post\n  operationId: sendStepUpEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/billing/subscription\n  method: get\n  operationId: getBillingSubscription\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/api/billing/plans\n  method: get\n  operationId: getBillingPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/api/billing/checkout\n  method: post\n  operationId: createBillingCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/billing/refund-autopilot\n  method: post\n  operationId: requestAutopilotRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/billing/checkout-pack\n  method: post\n  operationId: createPagePackCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/api/billing/webhook\n  method: post\n  operationId: receiveStripeBillingEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId:\
  \ mcpRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: options\n  operationId: mcpCorsPreflight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{id}/result\n  method: get\n  operationId: getDocumentResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statement-sets\n  method: post\n  operationId: createStatementSet\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/statement-sets/{id}\n  method: get\n  operationId: getStatementSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statement-sets/{id}/export\n  method: get\n  operationId: exportStatementSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schemas\n  method: post\n  operationId: createSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/schemas\n  method: get\n  operationId: listSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schemas/{id}\n  method: get\n  operationId: getSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schemas/{id}\n  method: put\n  operationId: updateSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schemas/{id}\n  method: delete\n  operationId: deleteSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chart-of-accounts\n  method: get\n  operationId: listChartOfAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chart-of-accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chart-of-accounts/import\n  method: post\n  operationId: importChartOfAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chart-of-accounts/sync\n  method: post\n  operationId: syncChartOfAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chart-of-accounts/settings\n  method: get\n  operationId: getCategorizationSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/chart-of-accounts/settings\n  method: patch\n  operationId: updateCategorizationSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chart-of-accounts/{id}\n  method: patch\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chart-of-accounts/{id}/archive\n  method: post\n  operationId: archiveAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/category-rules\n  method:\
  \ get\n  operationId: listCategoryRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/category-rules\n  method: post\n  operationId: createCategoryRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/category-rules/{id}\n  method: patch\n  operationId: updateCategoryRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/category-rules/{id}\n  method: delete\n  operationId: deleteCategoryRule\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/statement-sets/{id}/categorization\n  method: get\n  operationId: getStatementSetCategorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statement-sets/{id}/categorize\n  method: post\n  operationId: categorizeStatementSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/statement-sets/{id}/categorization/questions\n  method: get\n  operationId: getStatementSetCategorizationQuestions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statement-sets/{id}/categorization/groups\n  method: get\n  operationId: getStatementSetCategorizationGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statement-sets/{id}/categorization/groups/confirm\n  method: post\n  operationId: confirmStatementSetCategorizationGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/statement-sets/{id}/categorization/groups/undo\n  method: post\n  operationId: undoStatementSetCategorizationGroup\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/statement-sets/{id}/categorization/bulk\n  method: post\n  operationId: bulkUpdateStatementSetCategorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/statement-sets/{id}/categorization/accept-high-confidence\n  method: post\n  operationId: acceptHighConfidenceStatementSetCategorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /v1/statement-sets/{id}/categorization/rows/{documentId}/{rowIndex}\n  method: patch\n  operationId: updateStatementSetCategorizationRow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/statement-sets/{id}/categorization/rows/{documentId}/{rowIndex}/undo\n  method: post\n  operationId: undoStatementSetCategorizationRow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/statement-sets/{id}/deductions\n  method: get\n\
  \  operationId: getStatementSetDeductions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statement-sets/{id}/excluded\n  method: get\n  operationId: getStatementSetExcludedTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{id}/categorization\n  method: get\n  operationId: getDocumentCategorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{id}/categorization\n  method: patch\n  operationId: updateDocumentCategorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{id}/categorize\n  method: post\n  operationId: categorizeDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{id}/categorization/undo\n  method: post\n  operationId: undoDocumentCategorization\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/tax-years/{year}/categorized-transactions\n\
  \  method: get\n  operationId: getTaxYearCategorizedTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tax-years/{year}/vehicle-deduction\n  method: get\n  operationId: getTaxYearVehicleDeduction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tax-years/{year}/vehicle-deduction\n  method: patch\n  operationId: updateTaxYearVehicleDeduction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/year-overview\n  method: get\n  operationId: getYearOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tax-report\n  method: get\n  operationId: getTaxReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tax-report/export\n  method: get\n  operationId: exportTaxReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tax-report/transactions/{documentId}/{rowIndex}\n  method: patch\n  operationId: updateTaxReportTransactionCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /share/api/{token}\n  method: get\n  operationId: getSharedTaxReport\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /share/api/{token}/export\n  method: get\n  operationId: exportSharedTaxReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/form-1099\n  method: post\n  operationId: createForm1099Entry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/form-1099\n  method: get\n  operationId: listForm1099Entries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/form-1099/{id}\n  method: delete\n  operationId: deleteForm1099Entry\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/arkrel-com/agentic-access/arkrel-com-agentic-access.yml
summary_line: 88 operations · 51 acting · 2 human-in-the-loop
tags:
- Finance
- Bookkeeping
- Tax
- Software-as-a-Service
- Self-Employed
---
