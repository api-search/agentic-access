---
acting_count: 208
action_class_counts:
  acting: 208
  connected: 126
consequence_counts:
  physical: 8
  read: 126
  safety-critical: 23
  write: 177
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 23
kind: agentic-access
layout: agentic-access
method: generated
name: Dynamic Xyz Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /allowlists/{allowlistId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /environments/{environmentId}/gates/{gateId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/globalWallet/accessControl
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /environments/{environmentId}/globalWallet/accessControl
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /environments/{environmentId}/globalWallet/accessControl/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/globalWallet/accessControl/domains
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /environments/{environmentId}/globalWallet/accessControl/domains/{globalWalletAccessControlDomainId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /environments/{environmentId}/globalWallet/accessControl/enable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /environments/{environmentId}/globalWallet/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /environments/{environmentId}/integrations/chainalysis/sanctions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /environments/{environmentId}/nameService/{chainName}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/users/sessions/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/users/{userId}/sessions/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/waas/delegatedAccess/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /environments/{environmentId}/waas/{walletId}/delegatedAccess
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /organizations/{organizationId}/mfaSettings/{mfaDeviceType}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sdk/{environmentId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /sessions/{sessionId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /settings/exchanges/{exchangeId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /settings/providers/{providerId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /users/{userId}/mfa
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /users/{userId}/mfa/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /users/{userId}/sessions/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /members/{memberId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /members/{memberId}/delegateOwnership
operation_count: 334
overview: 'Dynamic exposes 334 API operations that an AI agent could call, of which 208 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 126 read, 177 write, 8 physical, and 23 safety-critical.


  23 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dynamic
provider_slug: dynamic-xyz
slug: dynamic-xyz-agentic-access
source_filename: dynamic-xyz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/dynamic-xyz-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 334\n  by_action_class:\n    acting: 208\n    connected: 126\n  by_consequence:\n    write: 177\n    read: 126\n    safety-critical: 23\n    physical: 8\n  human_in_the_loop_required: 23\noperations:\n- path: /environments/{environmentId}/globalWallet/settings\n  method: post\n  operationId: createGlobalWalletSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/globalWallet/settings\n\
  \  method: get\n  operationId: getGlobalWalletSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/globalWallet/settings\n  method: put\n  operationId: updateGlobalWalletSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/globalWallet/enable\n  method: put\n  operationId: enableGlobalWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/globalWallet/disable\n\
  \  method: put\n  operationId: disableGlobalWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/globalWallet/accessControl\n  method: get\n  operationId: getGlobalWalletAccessControlList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/globalWallet/accessControl\n  method: post\n  operationId: createGlobalWalletAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/globalWallet/accessControl\n  method: put\n  operationId: updateGlobalWalletAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/globalWallet/accessControl/enable\n  method: put\n  operationId: enableGlobalWalletAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/globalWallet/accessControl/disable\n\
  \  method: put\n  operationId: disableGlobalWalletAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/globalWallet/accessControl/domains\n  method: post\n  operationId: addGlobalWalletAccessControlDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/globalWallet/accessControl/domains/{globalWalletAccessControlDomainId}\n  method: delete\n  operationId: deleteGlobalWalletAccessControlDomainById\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/globalWallet/connections\n  method: get\n  operationId: getGlobalWalletConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/nameService/{chainName}\n  method: post\n  operationId: createNameService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/nameService/{chainName}\n\
  \  method: get\n  operationId: getNameService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/nameService/{chainName}\n  method: delete\n  operationId: deleteNameService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/nameService/{chainName}/signingMessage\n  method: post\n  operationId: fetchNameServiceSigningMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /environments/{environmentId}/nameService/{chainName}/enable\n  method: put\n  operationId: enableNameService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/nameService/{chainName}/disable\n  method: put\n  operationId: disableNameService\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/test/account\n  method: delete\n  operationId: deleteTestAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/test/account\n  method: get\n  operationId: getTestAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/test/account\n  method: post\n  operationId: createTestAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/custom/hostnames/{customHostnameId}\n  method: delete\n  operationId: deleteCustomHostname\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/custom/hostnames\n  method: get\n  operationId: getCustomHostnames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/custom/hostnames\n  method: post\n  operationId: createCustomHostname\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/exports\n  method: get\n  operationId: getEnvironmentExports\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/exports\n  method: post\n  operationId: createExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/exports/{exportId}/download\n  method: get\n  operationId: downloadExportById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/exports/{exportId}\n  method: get\n  operationId: getExportById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/gates\n\
  \  method: get\n  operationId: getEnvironmentGates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/gates\n  method: post\n  operationId: createGate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/gates/{gateId}\n  method: get\n  operationId: getGate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/gates/{gateId}\n  method: put\n  operationId: updateGate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/gates/{gateId}\n  method: delete\n  operationId: deleteGate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/gates/{gateId}/enable\n  method: put\n  operationId: enableGate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/gates/{gateId}/disable\n  method: put\n\
  \  operationId: disableGate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/settings/exchanges\n  method: get\n  operationId: getEnvironmentExchanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/settings/exchanges\n  method: post\n  operationId: createExchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/exchanges/{exchangeId}\n\
  \  method: get\n  operationId: getExchange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/exchanges/{exchangeId}\n  method: delete\n  operationId: deleteExchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/exchanges/{exchangeId}/enable\n  method: put\n  operationId: enableExchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/exchanges/{exchangeId}/disable\n  method: put\n  operationId:\
  \ disableExchange\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/settings/providers\n  method: get\n  operationId: getEnvironmentProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/settings/providers\n  method: post\n  operationId: createProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/settings/providers/urls\n\
  \  method: get\n  operationId: getEnvironmentProviderUrls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/providers/{providerId}\n  method: get\n  operationId: getProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/providers/{providerId}\n  method: put\n  operationId: updateProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/providers/{providerId}\n  method: delete\n  operationId: deleteProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/providers/{providerId}/enable\n  method: put\n  operationId: enableProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/providers/{providerId}/disable\n  method: put\n  operationId: disableProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/analytics/wallets\n\
  \  method: get\n  operationId: getWalletsBreakdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/analytics/visits\n  method: get\n  operationId: getVisitAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/analytics/overview\n  method: get\n  operationId: getAnalyticsOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/analytics/topline\n  method: get\n  operationId: getAnalyticsTopline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/analytics/engagement\n\
  \  method: get\n  operationId: getAnalyticsEngagement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/analytics/walletsBreakdown\n  method: get\n  operationId: getAnalyticsWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: post\n  operationId: createOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations\n  method: get\n  operationId: getOrganizationsForMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/billing/subscription\n  method: get\n  operationId: getBillingSubscriptionByOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/billing/upgrade\n  method: put\n  operationId: upgradeSubscriptionForOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/billing/subscription/coupon\n  method: put\n  operationId: applyCouponForSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}\n  method: get\n  operationId: getOrganizationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}\n  method: put\n  operationId: updateOrganizationById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/address\n  method: put\n  operationId: updateOrganizationAddressById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/ssoProvider\n  method: get\n  operationId: getSsoProviderForOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/ssoProvider\n  method: post\n  operationId: createSsoProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/ssoProvider/{ssoProviderId}\n  method: put\n  operationId: updateSsoProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/ssoProvider/{ssoProviderId}\n  method: delete\n  operationId: deleteSsoProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n  method: get\n  operationId: getProjectById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}\n  method: put\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n  method: delete\n  operationId: deleteProjectById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/projects\n  method: get\n  operationId: getProjects\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/customNetworks\n  method: get\n  operationId: getCustomNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/customNetworks\n  method: post\n  operationId: createCustomNetwork\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/customNetworks/{networkId}\n  method: get\n  operationId: getCustomNetwork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/customNetworks/{networkId}\n\
  \  method: put\n  operationId: updateCustomNetwork\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organizationId}/customNetworks/{networkId}\n  method: delete\n  operationId: deleteCustomNetwork\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/integrations/chainalysis\n  method: get\n  operationId: getChainalysisByEnvironmentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /environments/{environmentId}/integrations/chainalysis/sanctions/enable\n  method: put\n  operationId: enableSanctionsApiByEnvironmentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/integrations/chainalysis/sanctions/disable\n  method: put\n  operationId: disableSanctionsApiByEnvironmentId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}\n  method: get\n  operationId: getEnvironmentById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}\n  method: put\n  operationId: updateProjectSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/statistics/visitors\n  method: get\n  operationId: getVisitorsCountByEnvironmentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/keys\n  method: get\n  operationId: getKeysForEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/environments\n\
  \  method: get\n  operationId: getEnvironmentsByProjectId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{sessionId}/revoke\n  method: put\n  operationId: revokeSessionById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /environments/{environmentId}/embeddedWallets\n  method: post\n  operationId: createEmbeddedWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/embeddedWalletVersions\n\
  \  method: get\n  operationId: getActiveEmbeddedWalletVersionsForEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/embeddedWallets/farcaster\n  method: post\n  operationId: createEmbeddedWalletFromFarcaster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/wallets\n  method: post\n  operationId: createWalletLegacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /users/{userId}/wallets\n  method: get\n  operationId: getWalletsByUserIdLegacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/users/{userId}/balances\n  method: post\n  operationId: getUserAccountBalances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/users/{userId}/wallets\n  method: post\n  operationId: createWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /environments/{environmentId}/users/{userId}/wallets\n  method: get\n  operationId: getWalletsByUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{walletId}\n  method: get\n  operationId: getWalletByIdLegacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wallets/{walletId}\n  method: delete\n  operationId: deleteWalletByIdLegacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/wallets\n  method: get\n  operationId: getWalletsByEnvironmentId\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/wallets/{walletId}\n  method: get\n  operationId: getWalletById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/wallets/{walletId}\n  method: delete\n  operationId: deleteWalletById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-t\n\n# --- truncated at 32 KB (106 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/dynamic-xyz/refs/heads/main/agentic-access/dynamic-xyz-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic-xyz/refs/heads/main/agentic-access/dynamic-xyz-agentic-access.yml
summary_line: 334 operations · 208 acting · 23 human-in-the-loop
tags:
- Web3
- Wallets
- Authentication
- Embedded Wallets
- MPC
---
