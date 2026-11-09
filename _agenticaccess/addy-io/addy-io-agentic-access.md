---
acting_count: 82
action_class_counts:
  acting: 82
  connected: 22
api_specs:
- filename: addy-io-account-details-api-openapi.yml
  format: yaml
  label: addy.io Account Details API
  slug: addy-io-account-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-account-details-api-openapi.yml
- filename: addy-io-account-notifications-api-openapi.yml
  format: yaml
  label: addy.io Account Notifications API
  slug: addy-io-account-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-account-notifications-api-openapi.yml
- filename: addy-io-alias-bulk-actions-api-openapi.yml
  format: yaml
  label: addy.io Alias Bulk Actions API
  slug: addy-io-alias-bulk-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-alias-bulk-actions-api-openapi.yml
- filename: addy-io-aliases-api-openapi.yml
  format: yaml
  label: addy.io Aliases API
  slug: addy-io-aliases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-aliases-api-openapi.yml
- filename: addy-io-api-token-api-openapi.yml
  format: yaml
  label: addy.io API Token API
  slug: addy-io-api-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-api-token-api-openapi.yml
- filename: addy-io-app-version-api-openapi.yml
  format: yaml
  label: addy.io App Version API
  slug: addy-io-app-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-app-version-api-openapi.yml
- filename: addy-io-blocklist-api-openapi.yml
  format: yaml
  label: addy.io Blocklist API
  slug: addy-io-blocklist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-blocklist-api-openapi.yml
- filename: addy-io-domain-options-api-openapi.yml
  format: yaml
  label: addy.io Domain Options API
  slug: addy-io-domain-options-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-domain-options-api-openapi.yml
- filename: addy-io-domains-api-openapi.yml
  format: yaml
  label: addy.io Domains API
  slug: addy-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-domains-api-openapi.yml
- filename: addy-io-endpoints-api-openapi.yml
  format: yaml
  label: addy.io Endpoints API
  slug: addy-io-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-endpoints-api-openapi.yml
- filename: addy-io-failed-deliveries-api-openapi.yml
  format: yaml
  label: addy.io Failed Deliveries API
  slug: addy-io-failed-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-failed-deliveries-api-openapi.yml
- filename: addy-io-labels-api-openapi.yml
  format: yaml
  label: addy.io Labels API
  slug: addy-io-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-labels-api-openapi.yml
- filename: addy-io-recipients-api-openapi.yml
  format: yaml
  label: addy.io Recipients API
  slug: addy-io-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-recipients-api-openapi.yml
- filename: addy-io-rules-api-openapi.yml
  format: yaml
  label: addy.io Rules API
  slug: addy-io-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-rules-api-openapi.yml
- filename: addy-io-usernames-api-openapi.yml
  format: yaml
  label: addy.io Usernames API
  slug: addy-io-usernames-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addy-io/openapi/addy-io-usernames-api-openapi.yml
consequence_counts:
  physical: 7
  read: 22
  safety-critical: 10
  write: 65
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Addy Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/attached-recipients-only/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/catch-all-domains/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/catch-all-usernames/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/default-attached-recipients-only-domains/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/encrypted-recipients/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/inline-encrypted-recipients/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/protected-headers-recipients/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/remove-pgp-keys-recipients/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/remove-pgp-signatures-recipients/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/shared-with-family-domains/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/allowed-recipients
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/allowed-recipients/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/attached-recipients-only
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/domains/{id}/check-sending
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/failed-deliveries/{id}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/recipients/email/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/reorder-rules
operation_count: 104
overview: 'addy.io exposes 104 API operations that an AI agent could call, of which 82 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 65 write, 7 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: addy.io
provider_slug: addy-io
slug: addy-io-agentic-access
source_filename: addy-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/addy-io-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 104\n  by_action_class:\n    connected: 22\n    acting: 82\n  by_consequence:\n    read: 22\n    write: 65\n    physical: 7\n    safety-critical: 10\n  human_in_the_loop_required: 10\noperations:\n- path: /api/v1/api-token-details\n  method: get\n  operationId: getDetailsAboutTheCurrentAPIToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account-details\n  method: get\n  operationId: getAllAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account-notifications\n  method: get\n  operationId: getAllAccountNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/aliases/get/bulk\n  method: post\n  operationId: bulkGetSpecificAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/activate/bulk\n  method: post\n  operationId: bulkActivateSpecificAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /api/v1/aliases/deactivate/bulk\n  method: post\n  operationId: bulkDeactivateSpecificAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/pin/bulk\n  method: post\n  operationId: bulkPinSpecificAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/unpin/bulk\n  method: post\n  operationId: bulkUnpinSpecificAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/delete/bulk\n  method: post\n  operationId: bulkDeleteSpecificAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/restore/bulk\n  method: post\n  operationId: bulkRestoreSpecificAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/forget/bulk\n  method: post\n  operationId: bulkForgetSpecificAliases\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/recipients/bulk\n  method: post\n  operationId: bulkUpdateRecipientsForSpecificAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/labels/bulk\n  method: post\n  operationId: bulkUpdateLabelsForSpecificAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/aliases\n  method: get\n  operationId: getAllAliases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/aliases\n  method: post\n  operationId: createNewAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/{id}\n  method: get\n  operationId: getASpecificAlias\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/aliases/{id}\n  method: patch\n  operationId: updateASpecificAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/{id}\n  method: delete\n  operationId: deleteASpecificAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/{id}/restore\n  method: patch\n  operationId: restoreASpecificDeletedAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/aliases/{id}/forget\n  method: delete\n  operationId: forgetASpecificAlias\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/active-aliases\n  method: post\n  operationId: activateASpecificAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/active-aliases/{id}\n  method: delete\n  operationId: deactivateASpecificAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/pinned-aliases\n  method: post\n  operationId: pinASpecificAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pinned-aliases/{id}\n  method: delete\n  operationId: unpinASpecificAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/attached-recipients-only\n  method: post\n  operationId: limitTheRecipientsThatCanReplysendFromThisAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/attached-recipients-only/{id}\n  method: delete\n  operationId: disableTheLimitOfRecipientsThatCanReplysendFromThisAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/alias-recipients\n  method: post\n  operationId: updateRecipientsForASpecificAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /api/v1/alias-labels\n  method: post\n  operationId: updateLabelsForASpecificAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app-version\n  method: get\n  operationId: getTheCurrentAddyioAppVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/blocklist\n  method: get\n  operationId: getAllBlocklistEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/blocklist\n  method: post\n  operationId: createNewBlocklistEntry\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/blocklist/store/bulk\n  method: post\n  operationId: bulkCreateBlocklistEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/blocklist/delete/bulk\n  method: post\n  operationId: bulkDeleteBlocklistEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/blocklist/{id}\n  method:\
  \ delete\n  operationId: deleteASpecificBlocklistEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/domain-options\n  method: get\n  operationId: getDomainOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/domains\n  method: get\n  operationId: getAllDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/domains\n  method: post\n  operationId: createNewDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/domains/{id}\n  method: get\n  operationId: getASpecificDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/domains/{id}\n  method: patch\n  operationId: updateASpecificDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/domains/{id}\n  method: delete\n  operationId: deleteASpecificDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/domains/{id}/default-recipient\n  method: patch\n  operationId: updateDefaultRecipientForASpecificDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/domains/{id}/check-sending\n  method: post\n  operationId: checkDomainSendingRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/active-domains\n  method: post\n  operationId: activateASpecificDomain\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/active-domains/{id}\n  method: delete\n  operationId: deactivateASpecificDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/catch-all-domains\n  method: post\n  operationId: enableCatchAllForASpecificDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/catch-all-domains/{id}\n  method: delete\n  operationId: disableCatchAllForASpecificDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/default-attached-recipients-only-domains\n  method: post\n  operationId: limitNewAliasesOnADomainToAttachedRecipients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/default-attached-recipients-only-domains/{id}\n  method: delete\n  operationId: stopLimitingNewAliasesOnADomainToAttachedRecipients\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/shared-with-family-domains\n  method: post\n  operationId: shareADomainWithFamilyPlanMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/shared-with-family-domains/{id}\n  method: delete\n  operationId: stopSharingADomainWithFamilyPlanMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/internal/blocklist-check\n  method: get\n  operationId: checkIfTheGivenFromAddressorDomainIsBlockedForTheRecipientsUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/failed-deliveries\n  method: get\n  operationId: getAllFailedDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/failed-deliveries/{id}\n  method: get\n  operationId: getASpecificFailedDelivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/failed-deliveries/{id}\n  method: delete\n  operationId: deleteASpecificFailedDelivery\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/failed-deliveries/delete/bulk\n  method: post\n  operationId: bulkDeleteFailedDeliveries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/failed-deliveries/{id}/download\n  method: get\n  operationId: downloadASpecificFailedDelivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/failed-deliveries/{id}/resend\n  method: post\n  operationId: resendASpecificFailedDelivery\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/labels\n  method: get\n  operationId: getAllLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/labels\n  method: post\n  operationId: createNewLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/labels/{id}\n  method: get\n  operationId: getASpecificLabel\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/labels/{id}\n  method: patch\n  operationId: updateASpecificLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/labels/{id}\n  method: delete\n  operationId: deleteASpecificLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recipients\n  method: get\n  operationId: getAllRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recipients\n  method: post\n  operationId: createNewRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recipients/{id}\n  method: get\n  operationId: getASpecificRecipient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/recipients/{id}\n  method: patch\n  operationId: updateASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/recipients/{id}\n  method: delete\n  operationId: deleteASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recipients/email/resend\n  method: post\n  operationId: resendTheVerificationEmailForARecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recipient-keys/{id}\n  method: patch\n  operationId: addPublicKeyForASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recipient-keys/{id}\n  method: delete\n  operationId: removePublicKeyForASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/encrypted-recipients\n  method: post\n  operationId: enableEncryptionForASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/encrypted-recipients/{id}\n\
  \  method: delete\n  operationId: disableEncryptionForASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/inline-encrypted-recipients\n  method: post\n  operationId: enableInlinePGPInlineEncryptionForASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inline-encrypted-recipients/{id}\n  method: delete\n  operationId: disableInlinePGPInlineEncryptionForASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/protected-headers-recipients\n  method: post\n  operationId: enableProtectedHeadershideSubjectForASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/protected-headers-recipients/{id}\n  method: delete\n  operationId: disableProtectedHeadershideSubjectForASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/remove-pgp-keys-recipients\n  method: post\n  operationId: enableRemovePGPKeysForASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/remove-pgp-keys-recipients/{id}\n  method: delete\n  operationId: disableRemovePGPKeysForASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/remove-pgp-signatures-recipients\n  method: post\n  operationId: enableRemovePGPSignaturesForASpecificRecipient\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/remove-pgp-signatures-recipients/{id}\n  method: delete\n  operationId: disableRemovePGPSignaturesForASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/allowed-recipients\n  method: post\n  operationId: allowASpecificRecipientToReplysendFromYourAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n   \
  \   exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/allowed-recipients/{id}\n  method: delete\n  operationId: disallowASpecificRecipientToReplysendFromYourAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/active-recipients\n  method: post\n  operationId: activateASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/active-recipients/{id}\n  method: delete\n  operationId: deactivateASpecificRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/rules\n  method: get\n  operationId: getAllRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rules\n  method: post\n  operationId: createNewRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/rules/{id}\n  method: get\n  operationId:\
  \ getASpecificRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rules/{id}\n  method: patch\n  operationId: updateASpecificRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/rules/{id}\n  method: delete\n  operationId: deleteASpecificRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reorder-rules\n  method: post\n  operationId: updateTheOrderOfTheRules\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/active-rules\n  method: post\n  operationId: activateASpecificRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/active-rules/{id}\n  method: delete\n  operationId: deactivateASpecificRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/usernames\n  method: get\n  operationId: getAllUsernames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usernames\n  method: post\n  operationId: createNewUsername\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/usernames/{id}\n  method: get\n  operationId: getASpecificUsername\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (35 KB total) ---\n# Full source: https://artifacts.apis.io/addy-io/agentic-access/addy-io-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/addy-io/agentic-access/addy-io-agentic-access.yml
summary_line: 104 operations · 82 acting · 10 human-in-the-loop
tags:
- Company
- Email
- Address
- Software-as-a-Service
- Web App
---
