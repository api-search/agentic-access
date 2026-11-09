---
acting_count: 50
action_class_counts:
  acting: 50
  connected: 32
api_specs:
- filename: chartlink-app-account-api-openapi.yml
  format: yaml
  label: Chartlink Account API
  slug: chartlink-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-account-api-openapi.yml
- filename: chartlink-app-asset-types-api-openapi.yml
  format: yaml
  label: Chartlink Asset Types API
  slug: chartlink-app-asset-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-asset-types-api-openapi.yml
- filename: chartlink-app-assets-api-openapi.yml
  format: yaml
  label: Chartlink Assets API
  slug: chartlink-app-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-assets-api-openapi.yml
- filename: chartlink-app-billing-api-openapi.yml
  format: yaml
  label: Chartlink Billing API
  slug: chartlink-app-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-billing-api-openapi.yml
- filename: chartlink-app-billing-info-api-openapi.yml
  format: yaml
  label: Chartlink Billing Info API
  slug: chartlink-app-billing-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-billing-info-api-openapi.yml
- filename: chartlink-app-brands-api-openapi.yml
  format: yaml
  label: Chartlink Brands API
  slug: chartlink-app-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-brands-api-openapi.yml
- filename: chartlink-app-checkout-link-api-openapi.yml
  format: yaml
  label: Chartlink Checkout Link API
  slug: chartlink-app-checkout-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-checkout-link-api-openapi.yml
- filename: chartlink-app-data-api-openapi.yml
  format: yaml
  label: Chartlink Data API
  slug: chartlink-app-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-data-api-openapi.yml
- filename: chartlink-app-feedback-api-openapi.yml
  format: yaml
  label: Chartlink Feedback API
  slug: chartlink-app-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-feedback-api-openapi.yml
- filename: chartlink-app-fonts-api-openapi.yml
  format: yaml
  label: Chartlink Fonts API
  slug: chartlink-app-fonts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-fonts-api-openapi.yml
- filename: chartlink-app-geographies-api-openapi.yml
  format: yaml
  label: Chartlink Geographies API
  slug: chartlink-app-geographies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-geographies-api-openapi.yml
- filename: chartlink-app-invites-api-openapi.yml
  format: yaml
  label: Chartlink Invites API
  slug: chartlink-app-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-invites-api-openapi.yml
- filename: chartlink-app-keys-api-openapi.yml
  format: yaml
  label: Chartlink Keys API
  slug: chartlink-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-keys-api-openapi.yml
- filename: chartlink-app-oembed-api-openapi.yml
  format: yaml
  label: Chartlink Oembed API
  slug: chartlink-app-oembed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-oembed-api-openapi.yml
- filename: chartlink-app-signup-api-openapi.yml
  format: yaml
  label: Chartlink Signup API
  slug: chartlink-app-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-signup-api-openapi.yml
- filename: chartlink-app-try-api-openapi.yml
  format: yaml
  label: Chartlink Try API
  slug: chartlink-app-try-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-try-api-openapi.yml
- filename: chartlink-app-whoami-api-openapi.yml
  format: yaml
  label: Chartlink Whoami API
  slug: chartlink-app-whoami-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-whoami-api-openapi.yml
- filename: chartlink-app-workspace-api-openapi.yml
  format: yaml
  label: Chartlink Workspace API
  slug: chartlink-app-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartlink-app/openapi/chartlink-app-workspace-api-openapi.yml
consequence_counts:
  physical: 2
  read: 32
  safety-critical: 6
  write: 42
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Chartlink App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/account/connectors/{clientId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/assets/{id}/edit-links/{tokenId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/assets/{id}/preview-links/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/brands/{idOrSlug}/invites/{inviteId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/workspace/invites/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/assets/{id}/data-upload
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/checkout-link
operation_count: 82
overview: 'Chartlink exposes 82 API operations that an AI agent could call, of which 50 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 42 write, 2 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chartlink
provider_slug: chartlink-app
slug: chartlink-app-agentic-access
source_filename: chartlink-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/chartlink-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 82\n  by_action_class:\n    connected: 32\n    acting: 50\n  by_consequence:\n    read: 32\n    write: 42\n    safety-critical: 6\n    physical: 2\n  human_in_the_loop_required: 6\noperations:\n- path: /api/oembed\n  method: get\n  operationId: oembed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/webhook\n  method: post\n  operationId: paddleWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/signup\n  method: post\n  operationId: signup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/whoami\n  method: get\n  operationId: whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys/{id}\n  method: delete\n  operationId: revokeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/billing-info\n  method: get\n  operationId: getBilling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/checkout-link\n  method: post\n  operationId: createCheckoutLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/fonts\n  method: get\n  operationId: loadFont\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/fonts/catalog\n  method: get\n  operationId: listFonts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/geographies\n  method: get\n  operationId: listGeographies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/geographies/detect\n  method: post\n  operationId: detectGeography\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/geographies/requests\n  method: post\n  operationId: requestGeography\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/geographies/{id}\n  method: get\n  operationId: getGeography\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/geographies/{id}/data\n  method: get\n  operationId: getGeographyData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/data/tidy\n  method: post\n  operationId: tidyData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/assets\n  method: post\n  operationId: createAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}/restyle\n  method: post\n  operationId: restyleAsset\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}/premium\n  method: post\n  operationId: upgradeAssetToPremium\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/assets/{id}\n  method: patch\n  operationId: updateAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}/data\n  method: put\n  operationId: replaceAssetData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}/source\n  method: put\n  operationId: setAssetDataSource\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}/source\n  method: delete\n  operationId: clearAssetDataSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}/source/fetch\n  method: post\n  operationId: fetchAssetDataSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/assets/{id}/edit-link\n  method: post\n  operationId: createEditLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}/data-upload\n  method: post\n  operationId: createDataUploadLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}/preview-links/stop\n  method: post\n  operationId: stopPreviewLinks\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/assets/{id}/edit-links\n  method: get\n  operationId: listEditLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/assets/{id}/edit-links/{tokenId}\n  method: delete\n  operationId: revokeEditLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/assets/{id}/publish\n  method: post\n  operationId: publishAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/assets/{id}/unpublish\n  method: post\n  operationId: unpublishAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}/duplicate\n  method: post\n  operationId: duplicateAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}/restore\n  method: post\n  operationId: restoreAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{id}/versions\n  method: get\n  operationId: listAssetVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/assets/{id}/versions/{versionNumber}/restore\n  method: post\n  operationId: restoreAssetVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/brands/schema\n  method: get\n  operationId: getBrandTokensSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/brands\n  method: get\n  operationId: listBrands\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/brands\n  method: post\n  operationId: createBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/brands/{idOrSlug}\n  method: get\n  operationId: getBrand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/brands/{idOrSlug}\n  method: patch\n  operationId: updateBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/brands/{idOrSlug}\n  method: delete\n  operationId: deleteBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/brands/{idOrSlug}/guide\n  method: get\n  operationId: brandGuide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/brands/{idOrSlug}/vet\n  method: post\n  operationId: vetBrandChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/brands/{idOrSlug}/preview\n  method: post\n  operationId: previewBrandExample\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/brands/{idOrSlug}/setup\n  method: post\n  operationId: setupBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/brands/{idOrSlug}/shares\n  method: get\n  operationId: listBrandShares\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/brands/{idOrSlug}/shares\n \
  \ method: post\n  operationId: shareBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/brands/{idOrSlug}/shares/{shareId}\n  method: delete\n  operationId: unshareBrand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/brands/{idOrSlug}/invites/{inviteId}\n  method: delete\n  operationId: revokeBrandInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/workspace\n  method: get\n  operationId: getWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/workspace\n  method: patch\n  operationId: renameWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/workspace/invites\n  method: post\n  operationId: inviteToWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/workspace/invites/{id}\n  method: delete\n  operationId: revokeWorkspaceInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/workspace/members/{userId}\n  method: patch\n  operationId: setMemberRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/workspace/members/{userId}\n  method: delete\n  operationId: removeMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/workspaces\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/claim\n  method: post\n  operationId: claimWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/connector\n  method: get\n  operationId: getConnectorRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/connector\n  method: post\n  operationId: chooseConnectorWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/connectors\n  method: get\n  operationId: listConnectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account/connectors/{clientId}\n  method: delete\n  operationId: disconnectConnector\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/invites/{token}\n  method: get\n  operationId: getInvite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invites/{token}/accept\n  method: post\n  operationId: acceptInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/asset-types\n  method: get\n  operationId: listAssetTypes\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/asset-types/{type}/schema\n  method: get\n  operationId: getAssetTypeSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/try/fonts\n  method: get\n  operationId: loadFont\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/try/fonts/catalog\n  method: get\n  operationId: listFonts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/try/read\n  method: post\n  operationId: tryReadData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/try/look\n  method: post\n  operationId: tryBrandFromScreenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/try/event\n  method: post\n  operationId: tryEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/try/keep\n  method: post\n  operationId: tryKeep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/try/looks\n  method: get\n  operationId: tryLooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/try/starter\n  method: get\n  operationId: tryStarter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/try/detect\n  method: post\n  operationId: tryDetectGeography\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/try/geographies/{id}/data\n  method: get\n  operationId: tryGeographyData\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/feedback\n  method: post\n  operationId: submitFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/feedback\n  method: get\n  operationId: listFeedback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/chartlink-app/agentic-access/chartlink-app-agentic-access.yml
summary_line: 82 operations · 50 acting · 6 human-in-the-loop
tags:
- Company
- Charts
- Branding
- Artificial Intelligence
- Marketing
- Visualization
---
