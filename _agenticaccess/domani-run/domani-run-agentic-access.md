---
acting_count: 141
action_class_counts:
  acting: 141
  connected: 104
api_specs:
- filename: domani-run-account-api-openapi.yml
  format: yaml
  label: Domani Account API
  slug: domani-run-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-account-api-openapi.yml
- filename: domani-run-api-tokens-api-openapi.yml
  format: yaml
  label: Domani API Tokens API
  slug: domani-run-api-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-api-tokens-api-openapi.yml
- filename: domani-run-auth-api-openapi.yml
  format: yaml
  label: Domani Auth API
  slug: domani-run-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-auth-api-openapi.yml
- filename: domani-run-authentication-api-openapi.yml
  format: yaml
  label: Domani Authentication API
  slug: domani-run-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-authentication-api-openapi.yml
- filename: domani-run-backorders-api-openapi.yml
  format: yaml
  label: Domani Backorders API
  slug: domani-run-backorders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-backorders-api-openapi.yml
- filename: domani-run-billing-api-openapi.yml
  format: yaml
  label: Domani Billing API
  slug: domani-run-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-billing-api-openapi.yml
- filename: domani-run-collaboration-api-openapi.yml
  format: yaml
  label: Domani Collaboration API
  slug: domani-run-collaboration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-collaboration-api-openapi.yml
- filename: domani-run-connect-api-openapi.yml
  format: yaml
  label: Domani Connect API
  slug: domani-run-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-connect-api-openapi.yml
- filename: domani-run-discovery-api-openapi.yml
  format: yaml
  label: Domani Discovery API
  slug: domani-run-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-discovery-api-openapi.yml
- filename: domani-run-dns-api-openapi.yml
  format: yaml
  label: Domani DNS API
  slug: domani-run-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-dns-api-openapi.yml
- filename: domani-run-domain-search-api-openapi.yml
  format: yaml
  label: Domani Domain Search API
  slug: domani-run-domain-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-domain-search-api-openapi.yml
- filename: domani-run-domains-api-openapi.yml
  format: yaml
  label: Domani Domains API
  slug: domani-run-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-domains-api-openapi.yml
- filename: domani-run-email-api-openapi.yml
  format: yaml
  label: Domani Email API
  slug: domani-run-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-email-api-openapi.yml
- filename: domani-run-mailzero-assistant-api-openapi.yml
  format: yaml
  label: Domani Mailzero Assistant API
  slug: domani-run-mailzero-assistant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-mailzero-assistant-api-openapi.yml
- filename: domani-run-marketplace-api-openapi.yml
  format: yaml
  label: Domani Marketplace API
  slug: domani-run-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-marketplace-api-openapi.yml
- filename: domani-run-notifications-api-openapi.yml
  format: yaml
  label: Domani Notifications API
  slug: domani-run-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-notifications-api-openapi.yml
- filename: domani-run-referrals-api-openapi.yml
  format: yaml
  label: Domani Referrals API
  slug: domani-run-referrals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-referrals-api-openapi.yml
- filename: domani-run-status-api-openapi.yml
  format: yaml
  label: Domani Status API
  slug: domani-run-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-status-api-openapi.yml
- filename: domani-run-tlds-api-openapi.yml
  format: yaml
  label: Domani TLDs API
  slug: domani-run-tlds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-tlds-api-openapi.yml
- filename: domani-run-verify-service-api-openapi.yml
  format: yaml
  label: Domani Verify Service API
  slug: domani-run-verify-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-verify-service-api-openapi.yml
- filename: domani-run-webhooks-api-openapi.yml
  format: yaml
  label: Domani Webhooks API
  slug: domani-run-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domani-run/openapi/domani-run-webhooks-api-openapi.yml
consequence_counts:
  physical: 22
  read: 104
  safety-critical: 11
  write: 108
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 11
kind: agentic-access
layout: agentic-access
method: generated
name: Domani Run Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/agents/identity/{slug}/tokens/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/assistant/devices
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/assistant/tasks/{id}/escalate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/domains/{domain}/dnssec
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/domains/{domain}/redirect
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/emails/{address}/credentials/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/sessions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/sessions/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/tokens/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/watchlist/{domain}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/workspaces/{id}/ownership-transfer/{transferId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/agents/provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/login
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/backorders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/backorders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/billing/card
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/billing/connect
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/billing/connect/payout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/deals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/domains/buy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/domains/sell/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/domains/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/domains/transfer-watch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/domains/{domain}/verify-service
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/emails/{address}/connector/verify
operation_count: 245
overview: 'Domani exposes 245 API operations that an AI agent could call, of which 141 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 104 read, 108 write, 22 physical, and 11 safety-critical.


  11 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Domani
provider_slug: domani-run
slug: domani-run-agentic-access
source_filename: domani-run-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/domani-run-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 245\n  by_action_class:\n    acting: 141\n    connected: 104\n  by_consequence:\n    write: 108\n    physical: 22\n    read: 104\n    safety-critical: 11\n  human_in_the_loop_required: 11\noperations:\n- path: /api/auth/register\n  method: post\n  operationId: registerUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/login\n  method: post\n  operationId: loginUser\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/verify\n  method: get\n  operationId: verifyMagicLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/handoff\n  method: post\n  operationId: createAuthHandoff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/handoff/redeem\n  method: post\n  operationId: redeemAuthHandoff\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me\n  method: put\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/activation\n  method: get\n  operationId: getActivation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/activation\n  method: put\n  operationId: updateActivationPreference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/contact\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/contact\n  method: put\n  operationId: setContact\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/me/resend-verification\n  method: post\n  operationId: resendEmailVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tlds\n  method: get\n  operationId: listTlds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/search\n  method: get\n  operationId: search\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/suggest\n  method: get\n  operationId: suggestDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/identity\n  method: post\n  operationId: claimIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/identity\n  method: get\n  operationId: listIdentities\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/identity/{slug}/tokens\n  method: get\n  operationId: listAgentTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/identity/{slug}/tokens\n  method: post\n  operationId: createAgentToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/identity/{slug}/tokens/{id}\n  method: delete\n  operationId: revokeAgentToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/agents/identity/{slug}\n  method: patch\n  operationId: updateIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/identity/{slug}\n  method: delete\n  operationId: releaseIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/provision\n  method: post\n  operationId: provisionAgent\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/backorders\n  method: post\n  operationId: createBackorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/backorders\n  method: get\n  operationId: listBackorders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/backorders/{id}\n  method: get\n  operationId: getBackorder\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/backorders/{id}\n  method: delete\n  operationId: cancelBackorder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/watchlist\n  method: post\n  operationId: watchDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/watchlist\n  method: get\n  operationId: listWatches\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/watchlist/{domain}\n  method: delete\n  operationId: unwatchDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/domains/buy\n  method: post\n  operationId: buyDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/dns\n  method: get\n  operationId: getDnsRecords\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/dns\n  method: put\n  operationId: setDnsRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/dnssec\n  method: get\n  operationId: getDnssecRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/dnssec\n  method: post\n  operationId: addDnssecRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/dnssec\n  method: delete\n  operationId: deleteDnssecRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/domains/{domain}/dns/snapshot\n  method: post\n  operationId: snapshotDns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/dns/restore\n  method: post\n  operationId: restoreDns\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/dns/clone\n  method: post\n  operationId: cloneDns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/nameservers\n  method: get\n  operationId: getNameservers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/nameservers\n  method: put\n  operationId: setNameservers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/connect\n  method: post\n  operationId: connectDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/connect\n  method: get\n  operationId: listConnectProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/status\n  method: get\n  operationId: getDomainStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/domains/{domain}/email/check\n  method: get\n  operationId: checkEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/email/deliverability\n  method: get\n  operationId: getEmailDeliverability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/verify\n  method: post\n  operationId: verifyConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/verify-service\n  method: post\n  operationId: verifyService\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/verify-service\n  method: get\n  operationId: listVerifyServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}\n  method: get\n  operationId: getDomainInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/settings\n  method: put\n  operationId: updateDomainSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/parking\n  method: put\n  operationId: updateParking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/redirect\n  method: put\n  operationId: setDomainRedirect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/redirect\n  method: delete\n  operationId: clearDomainRedirect\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/domains/{domain}/for-sale\n  method: put\n  operationId: createListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/for-sale\n  method: patch\n  operationId: updateListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/for-sale\n  method: delete\n\
  \  operationId: cancelListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/sell\n  method: post\n  operationId: sellDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/sell/verify\n  method: post\n  operationId: verifySellListing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/sell/status\n  method: get\n  operationId:\
  \ getSellStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deals\n  method: get\n  operationId: listDeals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deals\n  method: post\n  operationId: createDeal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/deals/{id}\n  method: get\n  operationId: getDeal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/deals/{id}\n\
  \  method: patch\n  operationId: provideEppCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/deals/{id}/invoice\n  method: get\n  operationId: getDealInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/negotiations\n  method: get\n  operationId: listNegotiations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/negotiations\n  method: post\n  operationId: makeOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/negotiations/{id}\n  method: get\n  operationId: getNegotiation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/negotiations/{id}\n  method: post\n  operationId: respondToNegotiation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/negotiations/{id}\n  method: delete\n  operationId: cancelNegotiation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/negotiations/{id}/finalize\n  method: post\n  operationId: finalizeNegotiation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/broker\n  method: get\n  operationId: listBrokerRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/broker\n  method: post\n  operationId: createBrokerRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/broker/{id}\n  method: get\n  operationId: getBrokerRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/broker/{id}\n  method: delete\n  operationId: cancelBrokerRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/broker/respond\n  method: get\n  operationId: getBrokerInquiryState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/broker/respond\n  method: post\n  operationId: respondToBrokerInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/notifications\n  method: get\n  operationId: listNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/notifications/count\n  method: get\n  operationId: getUnreadCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/notifications/{id}\n  method: patch\n  operationId: markNotificationRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/notifications/read-all\n  method: post\n  operationId: markAllNotificationsRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/notifications/preferences\n  method: get\n  operationId: getNotificationPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/notifications/preferences\n  method: put\n  operationId: updateNotificationPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/domains/{domain}/analytics\n  method: get\n  operationId: getParkingAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/auth-code\n  method: get\n  operationId: getAuthCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/transfer-away\n  method: get\n  operationId: getTransferAway\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/transfer-status\n  method: get\n  operationId: checkTransferStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/import\n  method:\
  \ post\n  operationId: importDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/import/verify\n  method: post\n  operationId: verifyImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/adoption-plan\n  method: get\n  operationId: planDomainAdoption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/transfer-check\n  method: get\n  operationId: checkTransferEligibility\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/transfer-watch\n  method: post\n  operationId: watchTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/transfer\n  method: post\n  operationId: transferDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/renew\n  method: post\n\
  \  operationId: renewDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/buy-aftermarket\n  method: post\n  operationId: buyAftermarket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/{domain}/profile\n  method: get\n  operationId: getPublicDomainProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/profile\n  method: post\n  operationId: researchPublicDomainProfile\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/whois\n  method: get\n  operationId: whoisLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/{domain}/og\n  method: get\n  operationId: getDomainOg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/dns-check\n  method: get\n  operationId: dnsCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/registration-dates\n  method: get\n  operationId:\
  \ registrationDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tokens\n  method: get\n  operationId: listTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tokens\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tokens/{id}\n  method: delete\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n \
  \     proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sessions\n  method: delete\n  operationId: revokeOtherSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/sessions/{id}\n  method: delete\n  operationId: revokeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n     \
  \ proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\n\n# --- truncated at 32 KB (72 KB total) ---\n# Full source: https://artifacts.apis.io/domani-run/agentic-access/domani-run-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/domani-run/agentic-access/domani-run-agentic-access.yml
summary_line: 245 operations · 141 acting · 11 human-in-the-loop
tags:
- Company
- Domain
- Email
- DNS
- Platform
---
