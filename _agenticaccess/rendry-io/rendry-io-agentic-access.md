---
acting_count: 46
action_class_counts:
  acting: 46
  connected: 36
api_specs:
- filename: rendry-io-accounts-api-openapi.yml
  format: yaml
  label: rendry-io Accounts API
  slug: rendry-io-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-accounts-api-openapi.yml
- filename: rendry-io-assets-api-openapi.yml
  format: yaml
  label: rendry-io Assets API
  slug: rendry-io-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-assets-api-openapi.yml
- filename: rendry-io-batch-tasks-api-openapi.yml
  format: yaml
  label: rendry-io Batch Tasks API
  slug: rendry-io-batch-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-batch-tasks-api-openapi.yml
- filename: rendry-io-capabilities-api-openapi.yml
  format: yaml
  label: rendry-io Capabilities API
  slug: rendry-io-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-capabilities-api-openapi.yml
- filename: rendry-io-components-api-openapi.yml
  format: yaml
  label: rendry-io Components API
  slug: rendry-io-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-components-api-openapi.yml
- filename: rendry-io-design-guide-api-openapi.yml
  format: yaml
  label: rendry-io Design Guide API
  slug: rendry-io-design-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-design-guide-api-openapi.yml
- filename: rendry-io-documents-api-openapi.yml
  format: yaml
  label: rendry-io Documents API
  slug: rendry-io-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-documents-api-openapi.yml
- filename: rendry-io-embed-api-openapi.yml
  format: yaml
  label: rendry-io Embed API
  slug: rendry-io-embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-embed-api-openapi.yml
- filename: rendry-io-files-api-openapi.yml
  format: yaml
  label: rendry-io Files API
  slug: rendry-io-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-files-api-openapi.yml
- filename: rendry-io-generations-api-openapi.yml
  format: yaml
  label: rendry-io Generations API
  slug: rendry-io-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-generations-api-openapi.yml
- filename: rendry-io-images-api-openapi.yml
  format: yaml
  label: rendry-io Images API
  slug: rendry-io-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-images-api-openapi.yml
- filename: rendry-io-mcp-api-openapi.yml
  format: yaml
  label: rendry-io MCP API
  slug: rendry-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-mcp-api-openapi.yml
- filename: rendry-io-presets-api-openapi.yml
  format: yaml
  label: rendry-io Presets API
  slug: rendry-io-presets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-presets-api-openapi.yml
- filename: rendry-io-principal-api-openapi.yml
  format: yaml
  label: rendry-io Principal API
  slug: rendry-io-principal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-principal-api-openapi.yml
- filename: rendry-io-render-api-openapi.yml
  format: yaml
  label: rendry-io Render API
  slug: rendry-io-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-render-api-openapi.yml
- filename: rendry-io-rendering-api-openapi.yml
  format: yaml
  label: rendry-io Rendering API
  slug: rendry-io-rendering-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-rendering-api-openapi.yml
- filename: rendry-io-templates-api-openapi.yml
  format: yaml
  label: rendry-io Templates API
  slug: rendry-io-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-templates-api-openapi.yml
- filename: rendry-io-u-api-openapi.yml
  format: yaml
  label: rendry-io U API
  slug: rendry-io-u-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-u-api-openapi.yml
- filename: rendry-io-user-api-openapi.yml
  format: yaml
  label: rendry-io User API
  slug: rendry-io-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendry-io/openapi/rendry-io-user-api-openapi.yml
consequence_counts:
  read: 36
  safety-critical: 13
  write: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 13
kind: agentic-access
layout: agentic-access
method: generated
name: Rendry Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /art/prepare
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /documents
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /embed/origins
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /embed/sessions/{session}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /presets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /presets/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /presets/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /presets/{id}/components
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /presets/{id}/current
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /presets/{id}/group
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /presets/{id}/share
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /presets/{id}/theme
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /user/api-keys/{id}
operation_count: 82
overview: 'rendry-io exposes 82 API operations that an AI agent could call, of which 46 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read, 33 write, and 13 safety-critical.


  13 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: rendry-io
provider_slug: rendry-io
slug: rendry-io-agentic-access
source_filename: rendry-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/rendry-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 82\n  by_action_class:\n    connected: 36\n    acting: 46\n  by_consequence:\n    read: 36\n    write: 33\n    safety-critical: 13\n  human_in_the_loop_required: 13\noperations:\n- path: /assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets\n  method: post\n  operationId: uploadAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/import\n  method: post\n  operationId: importAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{id}\n  method: delete\n  operationId: deleteAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch-tasks\n  method: post\n  operationId: createBatchTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch-tasks/preview\n  method: post\n  operationId: previewBatchTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch-tasks/{id}\n  method: get\n  operationId: getBatchTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch-tasks/{id}/archive\n  method: get\n  operationId: downloadBatchArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capabilities\n  method: get\n  operationId: getCapabilities\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /components\n  method: get\n  operationId: getComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /design-guide\n  method: get\n  operationId: getDesignGuide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /documents/{id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}\n  method: put\n  operationId: updateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{path}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generations\n  method: get\n  operationId: listGenerations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/extract-object\n  method: post\n  operationId: extractObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/palette\n  method: post\n  operationId: getImagePalette\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/remove-background\n  method: post\n  operationId: removeBackground\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/search\n  method: get\n  operationId: searchImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: callMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /presets\n \
  \ method: get\n  operationId: listPresets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /presets\n  method: post\n  operationId: createPreset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /presets/{id}\n  method: get\n  operationId: getPreset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /presets/{id}\n  method: patch\n  operationId: updatePreset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /presets/{id}\n  method: delete\n  operationId: deletePreset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /presets/{id}/components\n  method: post\n  operationId: addPresetComponents\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /presets/{id}/current\n  method: put\n  operationId:\
  \ setCurrentPreset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /presets/{id}/group\n  method: delete\n  operationId: deletePresetGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /presets/{id}/share\n  method: post\n  operationId: publishPreset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /presets/{id}/share\n  method: get\n  operationId: getPresetShare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /presets/{id}/theme\n  method: post\n  operationId: setPresetTheme\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /presets/{id}/versions\n  method: get\n  operationId: listPresetVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /render/async\n  method: post\n  operationId:\
  \ renderAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render/batch\n  method: post\n  operationId: renderBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render/document\n  method: post\n  operationId: renderDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render/preview\n\
  \  method: post\n  operationId: renderPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render/status/{id}\n  method: get\n  operationId: getRenderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /render/sync\n  method: post\n  operationId: renderSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/{id}\n  method: get\n  operationId: getTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/{id}/clone\n  method: post\n  operationId: cloneTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/limits\n  method: get\n  operationId: getUserLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/usage\n  method: get\n  operationId: getUserUsage\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /u/{token}\n  method: get\n  operationId: getPublicRender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/api-keys/{id}\n  method: delete\n  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/account/deletion\n  method: get\n  operationId: getAccountDeletion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/account/deletion\n  method: post\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render/completions\n  method: get\n  operationId: listRenderCompletions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /presets/{id}/inputs\n  method: get\n  operationId: getPresetInputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}/inputs\n  method: get\n  operationId: getDocumentInputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /render/subscriptions\n  method: get\n  operationId: listCompletionSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /render/subscriptions\n  method: post\n  operationId: subscribeRenderFinished\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render/subscriptions/{id}\n  method: delete\n  operationId: unsubscribeRenderFinished\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render/subscriptions/{id}/replay\n  method: post\n  operationId: replayRenderFinished\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account}/members\n  method: get\n  operationId: listAccountMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account}/members/{actor}\n  method: put\n  operationId: setAccountMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /accounts/{account}/members/{actor}\n  method: delete\n  operationId: removeAccountMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embed/origins\n  method: get\n  operationId: listEmbedOrigins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /embed/origins\n  method: put\n  operationId: setEmbedOrigin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /embed/sessions\n  method:\
  \ post\n  operationId: issueEmbedSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embed/sessions/{session}\n  method: delete\n  operationId: revokeEmbedSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /embed/sessions/{session}/editor\n  method: get\n  operationId: getEmbedEditor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /embed/sessions/{session}/redeem\n  method:\
  \ post\n  operationId: redeemEmbedSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /principal\n  method: get\n  operationId: getPrincipal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch-tasks/guest\n  method: post\n  operationId: createGuestBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch-tasks/guest/preview\n  method: post\n  operationId: previewGuestBatch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch-tasks/guest/{token}\n  method: get\n  operationId: getGuestBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch-tasks/guest/{token}/archive\n  method: get\n  operationId: downloadGuestBatchArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /embed/brand/logo\n  method: get\n  operationId: getEmbedBrandLogo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /import/pdf\n  method: post\n  operationId: importPdfPage\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads\n  method: post\n  operationId: createUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads/{token}\n  method: put\n  operationId: putUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/generate\n  method: post\n\
  \  operationId: generateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai-styles\n  method: post\n  operationId: aiStyle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /art/prepare\n  method: post\n  operationId: prepareArt\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n"
source_yaml_url: https://artifacts.apis.io/rendry-io/agentic-access/rendry-io-agentic-access.yml
summary_line: 82 operations · 46 acting · 13 human-in-the-loop
tags:
- Company
- Image Rendering
- PDF Generation
- Template Engine
- AI Integration
---
