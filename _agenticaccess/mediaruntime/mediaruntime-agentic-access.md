---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 36
api_specs:
- filename: mediaruntime-discovery-api-openapi.yml
  format: yaml
  label: MediaRuntime Discovery API
  slug: mediaruntime-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-discovery-api-openapi.yml
- filename: mediaruntime-job-results-api-openapi.yml
  format: yaml
  label: MediaRuntime Job Results API
  slug: mediaruntime-job-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-job-results-api-openapi.yml
- filename: mediaruntime-jobs-api-openapi.yml
  format: yaml
  label: MediaRuntime Jobs API
  slug: mediaruntime-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-jobs-api-openapi.yml
- filename: mediaruntime-media-analysis-api-openapi.yml
  format: yaml
  label: MediaRuntime Media Analysis API
  slug: mediaruntime-media-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-media-analysis-api-openapi.yml
- filename: mediaruntime-mediaruntime-api-api-openapi.yml
  format: yaml
  label: MediaRuntime API
  slug: mediaruntime-mediaruntime-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-mediaruntime-api-api-openapi.yml
- filename: mediaruntime-moderation-api-openapi.yml
  format: yaml
  label: MediaRuntime Moderation API
  slug: mediaruntime-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-moderation-api-openapi.yml
- filename: mediaruntime-recipes-api-openapi.yml
  format: yaml
  label: MediaRuntime Recipes API
  slug: mediaruntime-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-recipes-api-openapi.yml
- filename: mediaruntime-sandbox-api-openapi.yml
  format: yaml
  label: MediaRuntime Sandbox API
  slug: mediaruntime-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-sandbox-api-openapi.yml
- filename: mediaruntime-uploads-api-openapi.yml
  format: yaml
  label: MediaRuntime Uploads API
  slug: mediaruntime-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-uploads-api-openapi.yml
- filename: mediaruntime-watermarks-api-openapi.yml
  format: yaml
  label: MediaRuntime Watermarks API
  slug: mediaruntime-watermarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-watermarks-api-openapi.yml
- filename: mediaruntime-webhooks-api-openapi.yml
  format: yaml
  label: MediaRuntime Webhooks API
  slug: mediaruntime-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-webhooks-api-openapi.yml
- filename: mediaruntime-marketplace-api-openapi.yml
  format: yaml
  label: MediaRuntime Marketplace API
  slug: mediaruntime-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-marketplace-api-openapi.yml
- filename: mediaruntime-sticker-collections-api-openapi.yml
  format: yaml
  label: MediaRuntime Sticker Collections API
  slug: mediaruntime-sticker-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-sticker-collections-api-openapi.yml
- filename: mediaruntime-sticker-runtime-api-openapi.yml
  format: yaml
  label: MediaRuntime Sticker Runtime API
  slug: mediaruntime-sticker-runtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/openapi/mediaruntime-sticker-runtime-api-openapi.yml
consequence_counts:
  read: 36
  safety-critical: 1
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Mediaruntime Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/sticker-collections/{collection_id}/packs/{pack_id}
operation_count: 61
overview: 'MediaRuntime exposes 61 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read, 24 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MediaRuntime
provider_slug: mediaruntime
slug: mediaruntime-agentic-access
source_filename: mediaruntime-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: generated\nsource: openapi/mediaruntime-discovery-api-openapi.yml, openapi/mediaruntime-job-results-api-openapi.yml,\n  openapi/mediaruntime-jobs-api-openapi.yml, openapi/mediaruntime-media-analysis-api-openapi.yml,\n  openapi/mediaruntime-moderation-api-openapi.yml, openapi/mediaruntime-openapi.json, openapi/mediaruntime-recipes-api-openapi.yml,\n  openapi/mediaruntime-sandbox-api-openapi.yml, openapi/mediaruntime-uploads-api-openapi.yml,\n  openapi/mediaruntime-watermarks-api-openapi.yml, openapi/mediaruntime-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 61\n  by_action_class:\n    connected: 36\n    acting: 25\n  by_consequence:\n    read: 36\n    write: 24\n    safety-critical:\
  \ 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/capabilities\n  method: get\n  operationId: getCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/bundle\n  method: get\n  operationId: downloadJobBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/jobs/{job_id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/codes\n  method: get\n  operationId: getCodeDetections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/compatibility-report\n  method: get\n  operationId: getCompatibilityReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/media-report\n  method: get\n  operationId: getMediaReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/moderation\n\
  \  method: get\n  operationId: getModerationResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/watermark-logo/confirm\n  method: post\n  operationId: confirmWatermarkLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/watermark-logo/upload-url\n  method: post\n  operationId: createWatermarkLogoUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/capabilities\n  method: get\n \
  \ operationId: getCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{job_id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/artifacts\n  method: get\n  operationId: listJobArtifacts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/artifacts/{artifact_id}/download\n  method: get\n  operationId: downloadJobArtifact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/bundle\n  method: get\n  operationId: downloadJobBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/clip-candidates\n  method: get\n  operationId: getClipCandidates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/codes\n  method: get\n  operationId: getCodeDetections\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/compatibility-report\n  method: get\n  operationId: getCompatibilityReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/media-report\n  method: get\n  operationId: getMediaReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/moderation\n  method: get\n  operationId: getModerationResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/retry-webhook\n  method: post\n  operationId: retryJobWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/marketplace/packs\n  method: get\n  operationId: listMarketplacePacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/marketplace/packs/{slug}\n  method: get\n  operationId: getMarketplacePack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recipes\n  method: get\n  operationId: listRecipes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recipes\n  method: post\n  operationId: createRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipes/{name}\n  method: delete\n  operationId: archiveRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipes/{name}\n  method: get\n  operationId: getRecipe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recipes/{name}/versions\n  method: post\n  operationId: createRecipeVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipes/{name}/versions/{version}\n  method: get\n  operationId: getRecipeVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sandbox/session\n  method: post\n  operationId: createSandboxSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sticker-collections\n  method: get\n  operationId: listStickerCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sticker-collections\n  method: post\n  operationId:\
  \ createStickerCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sticker-collections/{collection_id}\n  method: delete\n  operationId: archiveStickerCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sticker-collections/{collection_id}\n  method: get\n  operationId: getStickerCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sticker-collections/{collection_id}\n  method: patch\n\
  \  operationId: updateStickerCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sticker-collections/{collection_id}/packs\n  method: get\n  operationId: listStickerCollectionPackBindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sticker-collections/{collection_id}/packs\n  method: post\n  operationId: enableStickerCollectionActivation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sticker-collections/{collection_id}/packs/{pack_id}\n\
  \  method: delete\n  operationId: disableStickerCollectionPack\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sticker-collections/{collection_id}/packs/{pack_id}\n  method: put\n  operationId: enableStickerCollectionPack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sticker-runtime/client-tokens\n  method: post\n  operationId: createStickerRuntimeClientToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sticker-runtime/usage/current\n  method: get\n  operationId: getCurrentStickerRuntimeUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stickers/packs\n  method: get\n  operationId: listRuntimeStickerPacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stickers/search\n  method: get\n  operationId: searchRuntimeStickers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stickers/typeahead\n  method: get\n  operationId: typeaheadRuntimeStickers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stickers/{sticker_id}\n  method: get\n  operationId: getRuntimeSticker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stickers/{sticker_id}/assets/{variant}\n  method: get\n  operationId: resolveRuntimeStickerVariant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/upload-url\n  method: post\n  operationId: createUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipes\n  method: get\n  operationId: listRecipes\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recipes\n  method: post\n  operationId: createRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipes/{name}\n  method: delete\n  operationId: archiveRecipe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipes/{name}\n  method: get\n  operationId: getRecipe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recipes/{name}/versions\n  method: post\n  operationId: createRecipeVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipes/{name}/versions/{version}\n  method: get\n  operationId: getRecipeVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sandbox/session\n  method: post\n  operationId: createSandboxSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /v1/upload-url\n  method: post\n  operationId: createUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/watermark-logo/confirm\n  method: post\n  operationId: confirmWatermarkLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/watermark-logo/upload-url\n  method: post\n  operationId: createWatermarkLogoUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{job_id}/retry-webhook\n  method: post\n  operationId: retryJobWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediaruntime/refs/heads/main/agentic-access/mediaruntime-agentic-access.yml
summary_line: 61 operations · 25 acting · 1 human-in-the-loop
tags:
- Media Processing
- Video
- Audio
- Runtime
- Video Encoding
- Audio Processing
- Image Processing
- Content Moderation
- Media API
- Asynchronous Processing
---
