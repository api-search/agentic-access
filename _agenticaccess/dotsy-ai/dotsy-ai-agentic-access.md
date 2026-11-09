---
acting_count: 111
action_class_counts:
  acting: 111
  connected: 79
api_specs:
- filename: dotsy-ai-account-api-openapi.yml
  format: yaml
  label: dotsy Account API
  slug: dotsy-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-account-api-openapi.yml
- filename: dotsy-ai-assets-api-openapi.yml
  format: yaml
  label: dotsy Assets API
  slug: dotsy-ai-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-assets-api-openapi.yml
- filename: dotsy-ai-brief-api-openapi.yml
  format: yaml
  label: dotsy Brief API
  slug: dotsy-ai-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-brief-api-openapi.yml
- filename: dotsy-ai-collections-api-openapi.yml
  format: yaml
  label: dotsy Collections API
  slug: dotsy-ai-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-collections-api-openapi.yml
- filename: dotsy-ai-content-api-openapi.yml
  format: yaml
  label: dotsy Content API
  slug: dotsy-ai-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-content-api-openapi.yml
- filename: dotsy-ai-domains-api-openapi.yml
  format: yaml
  label: dotsy Domains API
  slug: dotsy-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-domains-api-openapi.yml
- filename: dotsy-ai-draft-publish-api-openapi.yml
  format: yaml
  label: dotsy Draft & publish API
  slug: dotsy-ai-draft-publish-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-draft-publish-api-openapi.yml
- filename: dotsy-ai-forms-api-openapi.yml
  format: yaml
  label: dotsy Forms API
  slug: dotsy-ai-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-forms-api-openapi.yml
- filename: dotsy-ai-guest-api-openapi.yml
  format: yaml
  label: dotsy Guest API
  slug: dotsy-ai-guest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-guest-api-openapi.yml
- filename: dotsy-ai-import-api-openapi.yml
  format: yaml
  label: dotsy Import API
  slug: dotsy-ai-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-import-api-openapi.yml
- filename: dotsy-ai-jobs-api-openapi.yml
  format: yaml
  label: dotsy Jobs API
  slug: dotsy-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-jobs-api-openapi.yml
- filename: dotsy-ai-members-api-openapi.yml
  format: yaml
  label: dotsy Members API
  slug: dotsy-ai-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-members-api-openapi.yml
- filename: dotsy-ai-pages-api-openapi.yml
  format: yaml
  label: dotsy Pages API
  slug: dotsy-ai-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-pages-api-openapi.yml
- filename: dotsy-ai-routes-api-openapi.yml
  format: yaml
  label: dotsy Routes API
  slug: dotsy-ai-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-routes-api-openapi.yml
- filename: dotsy-ai-sites-api-openapi.yml
  format: yaml
  label: dotsy Sites API
  slug: dotsy-ai-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-sites-api-openapi.yml
- filename: dotsy-ai-support-api-openapi.yml
  format: yaml
  label: dotsy Support API
  slug: dotsy-ai-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dotsy-ai/openapi/dotsy-ai-support-api-openapi.yml
consequence_counts:
  physical: 4
  read: 79
  safety-critical: 4
  write: 103
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Dotsy Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/account/keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/forms/unsubscribe/{token}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/sites/{slug}/forms/recipients/{email}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/sites/{slug}/shared-sections/suggestions/dismiss
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/sites/{slug}/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/sites/{slug}/transfer/{transferId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/support/conversations/{id}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/transfers/{token}/accept
operation_count: 190
overview: 'dotsy exposes 190 API operations that an AI agent could call, of which 111 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 79 read, 103 write, 4 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: dotsy
provider_slug: dotsy-ai
slug: dotsy-ai-agentic-access
source_filename: dotsy-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dotsy-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 190\n  by_action_class:\n    connected: 79\n    acting: 111\n  by_consequence:\n    read: 79\n    write: 103\n    safety-critical: 4\n    physical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /api/v1/sites\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites\n  method: post\n  operationId: createSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/me\n  method: get\n  operationId: getAccountMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/notifications/summary\n  method: get\n  operationId: getNotificationsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/notifications\n  method: get\n  operationId: listNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/notifications/read\n  method: post\n  operationId: markNotificationsRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/notifications/done\n  method: post\n  operationId: markNotificationsDone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/notifications/snooze\n  method: post\n  operationId: snoozeNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/manifest\n  method:\
  \ get\n  operationId: getSiteManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/preflight\n  method: post\n  operationId: preflightSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/search\n  method: get\n  operationId: searchContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/sites/{slug}/content/rename\n  method: post\n  operationId: renameContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/collections/schema\n  method: get\n  operationId: getCollectionSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/collections/schema\n  method: put\n  operationId: updateCollectionSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/sites/{slug}/collections/schema/infer\n  method: post\n  operationId: inferCollectionSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/collections/fields/set\n  method: post\n  operationId: setCollectionField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/collections/fields/rename\n  method: post\n  operationId: renameCollectionField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/collections/fields/undo\n  method: post\n  operationId: undoCollectionFieldEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/collections/export\n  method: get\n  operationId: exportCollectionCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/collections/items/status\n  method: post\n  operationId: setItemStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/boards\n  method: get\n  operationId: getBoard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/suggestions\n  method: get\n  operationId: listSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/suggestions/approve\n  method: post\n  operationId: approveSuggestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /api/v1/sites/{slug}/suggestions/merge\n  method: post\n  operationId: mergeSuggestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/suggestions/decline\n  method: post\n  operationId: declineSuggestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/ideas\n  method: post\n  operationId: addIdea\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/ideas\n  method: get\n  operationId: listIdeas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/votes\n  method: get\n  operationId: listVotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/votes\n  method: delete\n  operationId: removeVotes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/voters\n  method: delete\n  operationId: forgetVoter\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/helpful\n  method: get\n  operationId: getHelpfulSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/product-kit\n  method: post\n  operationId: installProductKit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/changeset\n  method: post\n  operationId: applyChangeset\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/content\n  method: get\n  operationId: listContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/content/{key}\n  method: get\n  operationId: getContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/content/{key}\n  method: put\n  operationId: putContent\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/content/{key}\n  method: delete\n  operationId: deleteContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/content-raw/{key}\n  method: put\n  operationId: putContentRaw\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/sites/{slug}/routes\n  method: get\n  operationId: listRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/routes/{path}\n  method: get\n  operationId: getRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/routes/{path}\n  method: put\n  operationId: putRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/routes/{path}\n  method: patch\n  operationId: patchRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/routes/{path}\n  method: delete\n  operationId: deleteRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/routes/rename\n  method: post\n  operationId: renameRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/assets/bulk\n  method: post\n  operationId: bulkPutAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/assets/optimize\n  method: post\n  operationId: optimizeAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/assets/{key}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/assets/{key}\n  method: put\n  operationId: putAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/assets/{key}\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/assets-raw/{key}\n  method: put\n  operationId: putAssetRaw\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/static-files/{path}\n  method: put\n  operationId: putStaticFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/static-files/{path}\n  method: delete\n  operationId: deleteStaticFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/verify\n  method: post\n  operationId: verifySite\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/draft-status\n  method: get\n  operationId: getDraftStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/revert\n  method: post\n  operationId: revertDrafts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/review\n  method: get\n  operationId: getReviewQueue\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/review/item\n  method: get\n  operationId: getReviewItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/review/ready\n  method: post\n  operationId: markReviewReady\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/review/unready\n  method: post\n  operationId: unmarkReviewReady\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/brief\n  method: get\n  operationId: getBrief\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/brief\n  method: put\n  operationId: updateBrief\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/custom-domains\n  method: get\n  operationId: listCustomDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/custom-domains\n  method: post\n  operationId: addCustomDomain\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/custom-domains/connect\n  method: get\n  operationId: getCustomDomainConnect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/custom-domains/connect/reapply-oauth\n  method: post\n  operationId: reapplyCustomDomainOauth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/custom-domains/{host}/refresh\n  method: post\n  operationId:\
  \ refreshCustomDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/custom-domains/{host}/provider-connect\n  method: post\n  operationId: connectCustomDomainProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/custom-domains/{host}/primary\n  method: post\n  operationId: setPrimaryCustomDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/custom-domains/{host}\n  method: delete\n  operationId: removeCustomDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/search-console/connect\n  method: post\n  operationId: connectSearchConsole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/search-console/managed\n  method: post\n  operationId: postSearchConsoleManaged\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/search-console\n  method: get\n  operationId: getSearchConsole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/search-console\n  method: delete\n  operationId: disconnectSearchConsole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/search-console/performance\n  method: get\n  operationId: getSearchPerformance\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/search-console/indexing\n  method: get\n  operationId: getSearchIndexing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/search-console/inspect\n  method: post\n  operationId: inspectUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/seo/opportunities\n  method: get\n  operationId: getSeoOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/custom-code\n\
  \  method: get\n  operationId: getCustomCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/custom-code\n  method: put\n  operationId: putCustomCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/access\n  method: get\n  operationId: getSiteAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/access\n  method: put\n  operationId: putSiteAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/form-submissions/export.csv\n  method: get\n  operationId: exportFormSubmissionsCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/form-submissions\n  method: get\n  operationId: listFormSubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/form-submissions/{id}\n  method: get\n  operationId: getFormSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/forms/recipients\n  method: get\n  operationId: listFormRecipients\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/forms/recipients/confirm-requests\n  method: post\n  operationId: requestFormRecipientConfirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/forms/recipients/{email}\n  method: delete\n  operationId: revokeFormRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/forms/confirm/{token}\n  method: get\n\
  \  operationId: getFormRecipientConfirm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/forms/confirm/{token}\n  method: post\n  operationId: confirmFormRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forms/unsubscribe/{token}\n  method: get\n  operationId: getFormRecipientUnsubscribe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/forms/unsubscribe/{token}\n  method: post\n  operationId: unsubscribeFormRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/sites/{slug}/activity\n  method: get\n  operationId: listActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/activity/{id}/diff\n  method: get\n  operationId: getActivityDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/activity/{id}/revert\n  method: post\n  operationId: revertActivityChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/versions\n  method: get\n  operationId: listVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/versions/{version}/changes\n  method: get\n  operationId: getVersionChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/versions/{version}/restore\n  method: post\n  operationId: restoreVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/versions/undo-last\n  method: post\n  operationId:\
  \ undoLastPublish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/shared-sections/analyze\n  method: post\n  operationId: analyzeSharedSection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/shared-sections/compare\n  method: post\n  operationId: compareSharedSection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sites/{slug}/shared-sections/suggestions\n  method:\
  \ get\n  operationId: listSharedSectionSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sites/{slug}/shared-sections/suggestions/dismiss\n  method: post\n  operationId: dismissSharedSectionSuggestion\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/sites/{slug}/shared-sections\n  method: get\n  operationId: listSharedSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (57 KB total) ---\n# Full source: https://artifacts.apis.io/dotsy-ai/agentic-access/dotsy-ai-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/dotsy-ai/agentic-access/dotsy-ai-agentic-access.yml
summary_line: 190 operations · 111 acting · 4 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Website Builder
- No-Code
- Free
---
