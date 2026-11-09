---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 20
api_specs:
- filename: klisten-co-kr-account-api-openapi.yml
  format: yaml
  label: klisten-co-kr Account API
  slug: klisten-co-kr-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-account-api-openapi.yml
- filename: klisten-co-kr-actioncheck-api-openapi.yml
  format: yaml
  label: klisten-co-kr Actioncheck API
  slug: klisten-co-kr-actioncheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-actioncheck-api-openapi.yml
- filename: klisten-co-kr-agentescrow-api-openapi.yml
  format: yaml
  label: klisten-co-kr Agentescrow API
  slug: klisten-co-kr-agentescrow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-agentescrow-api-openapi.yml
- filename: klisten-co-kr-agentscore-api-openapi.yml
  format: yaml
  label: klisten-co-kr Agentscore API
  slug: klisten-co-kr-agentscore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-agentscore-api-openapi.yml
- filename: klisten-co-kr-attestations-api-openapi.yml
  format: yaml
  label: klisten-co-kr Attestations API
  slug: klisten-co-kr-attestations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-attestations-api-openapi.yml
- filename: klisten-co-kr-checkout-api-openapi.yml
  format: yaml
  label: klisten-co-kr Checkout API
  slug: klisten-co-kr-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-checkout-api-openapi.yml
- filename: klisten-co-kr-cleargate-api-openapi.yml
  format: yaml
  label: klisten-co-kr Cleargate API
  slug: klisten-co-kr-cleargate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-cleargate-api-openapi.yml
- filename: klisten-co-kr-gate-api-openapi.yml
  format: yaml
  label: klisten-co-kr Gate API
  slug: klisten-co-kr-gate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-gate-api-openapi.yml
- filename: klisten-co-kr-health-api-openapi.yml
  format: yaml
  label: klisten-co-kr Health API
  slug: klisten-co-kr-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-health-api-openapi.yml
- filename: klisten-co-kr-metermcp-api-openapi.yml
  format: yaml
  label: klisten-co-kr Metermcp API
  slug: klisten-co-kr-metermcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-metermcp-api-openapi.yml
- filename: klisten-co-kr-modelroute-api-openapi.yml
  format: yaml
  label: klisten-co-kr Modelroute API
  slug: klisten-co-kr-modelroute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-modelroute-api-openapi.yml
- filename: klisten-co-kr-scans-api-openapi.yml
  format: yaml
  label: klisten-co-kr Scans API
  slug: klisten-co-kr-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-scans-api-openapi.yml
- filename: klisten-co-kr-services-api-openapi.yml
  format: yaml
  label: klisten-co-kr Services API
  slug: klisten-co-kr-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-services-api-openapi.yml
- filename: klisten-co-kr-toolrank-api-openapi.yml
  format: yaml
  label: klisten-co-kr Toolrank API
  slug: klisten-co-kr-toolrank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-toolrank-api-openapi.yml
- filename: klisten-co-kr-watches-api-openapi.yml
  format: yaml
  label: klisten-co-kr Watches API
  slug: klisten-co-kr-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-watches-api-openapi.yml
- filename: klisten-co-kr-webhooks-api-openapi.yml
  format: yaml
  label: klisten-co-kr Webhooks API
  slug: klisten-co-kr-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klisten-co-kr/openapi/klisten-co-kr-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 20
  safety-critical: 2
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Klisten Co Kr Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/account/actioncheck/policies/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/account/keys/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/topups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/topups/{id}/capture
operation_count: 46
overview: 'klisten-co-kr exposes 46 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 22 write, 2 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: klisten-co-kr
provider_slug: klisten-co-kr
slug: klisten-co-kr-agentic-access
source_filename: klisten-co-kr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/klisten-co-kr-models-openapi.json, openapi/klisten-co-kr-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    connected: 20\n    acting: 26\n  by_consequence:\n    read: 20\n    write: 22\n    physical: 2\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/modelroute/catalog\n  method: get\n  operationId: getModelRouteCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modelroute/select\n  method: post\n  operationId: selectDiscoveredModels\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/modelroute/decisions/{id}\n  method: get\n  operationId: getModelRouteDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agentscore/activity\n  method: post\n  operationId: issueCredentialActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agentscore/activity/{jobId}\n  method: get\n  operationId: readCredentialActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/metermcp/usage\n  method: get\n  operationId: getMeterLiveUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agentescrow/drafts\n  method: post\n  operationId: createEscrowDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agentescrow/drafts/{id}\n  method: get\n  operationId: getEscrowDraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cleargate/check\n  method: post\n  operationId: checkClearGateGrant\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/actioncheck/check\n  method: post\n  operationId: checkAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/config\n  method: get\n  operationId: getCheckoutConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout/topups\n  method: post\n  operationId: createCheckoutTopup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/topups/{id}\n  method: get\n  operationId: getCheckoutTopup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout/topups/{id}/approval\n  method: get\n  operationId: getCheckoutApproval\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout/topups/{id}/capture\n  method: post\n  operationId: captureCheckoutTopup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/paypal\n  method: post\n  operationId: receivePayPalWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/actioncheck/policies\n  method: get\n  operationId: listActionCheckPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/actioncheck/policies\n  method: post\n  operationId: createActionCheckPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/actioncheck/policies/{id}\n  method: delete\n  operationId: revokeActionCheckPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/account/config\n  method: get\n  operationId: getAccountConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/agentscore/enroll\n  method: post\n  operationId: enrollCredentialActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/cleargate/grants\n  method: post\n  operationId: createCustomerDocumentationGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/bootstrap\n  method: post\n  operationId: bootstrapAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/overview\n  method: get\n  operationId: getAccountOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/keys\n  method: post\n  operationId: createAccountKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/keys/{id}\n  method: delete\n  operationId: revokeAccountKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/account/keys/{id}/budget\n  method: put\n  operationId: setAccountKeyBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/budget\n  method: put\n  operationId: setAccountBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/toolrank/tools\n  method: get\n  operationId: listTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/toolrank/tools/{id}\n  method: get\n  operationId: getTool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/toolrank/select\n  method: post\n  operationId:\
  \ selectTools\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/toolrank/decisions/{id}\n  method: get\n  operationId: getToolRankDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{id}/trust\n  method: get\n  operationId: getServiceTrust\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/toolguard/services\n  method:\
  \ get\n  operationId: listToolguardServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/toolguard/services\n  method: post\n  operationId: registerToolguardService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/toolguard/services/{id}/baseline\n  method: post\n  operationId: approveToolguardBaseline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scans/paid\n  method: post\n  operationId:\
  \ createPaidScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scans\n  method: post\n  operationId: createScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scans/{id}\n  method: get\n  operationId: getScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gate/check\n  method: post\n  operationId: checkGate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gate/check-paid\n  method: post\n  operationId: checkPaidGate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watches\n  method: post\n  operationId: createWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watches/{id}\n  method: get\n  operationId: getWatch\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watches/{id}\n  method: delete\n  operationId: deleteWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attestations/{id}\n  method: get\n  operationId: getAttestation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/klisten-co-kr/agentic-access/klisten-co-kr-agentic-access.yml
summary_line: 46 operations · 26 acting · 2 human-in-the-loop
tags:
- Artificial Intelligence
- ToolGuard
- MCP
- Policy
- Prepaid
---
