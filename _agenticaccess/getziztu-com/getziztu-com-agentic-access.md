---
acting_count: 40
action_class_counts:
  acting: 40
  connected: 16
api_specs:
- filename: getziztu-com-characters-api-openapi.yml
  format: yaml
  label: getziztu-com Characters API
  slug: getziztu-com-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-characters-api-openapi.yml
- filename: getziztu-com-credits-api-openapi.yml
  format: yaml
  label: getziztu-com Credits API
  slug: getziztu-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-credits-api-openapi.yml
- filename: getziztu-com-director-api-openapi.yml
  format: yaml
  label: getziztu-com Director API
  slug: getziztu-com-director-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-director-api-openapi.yml
- filename: getziztu-com-export-api-openapi.yml
  format: yaml
  label: getziztu-com Export API
  slug: getziztu-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-export-api-openapi.yml
- filename: getziztu-com-generate-api-openapi.yml
  format: yaml
  label: getziztu-com Generate API
  slug: getziztu-com-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-generate-api-openapi.yml
- filename: getziztu-com-jobs-api-openapi.yml
  format: yaml
  label: getziztu-com Jobs API
  slug: getziztu-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-jobs-api-openapi.yml
- filename: getziztu-com-media-api-openapi.yml
  format: yaml
  label: getziztu-com Media API
  slug: getziztu-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-media-api-openapi.yml
- filename: getziztu-com-meta-api-openapi.yml
  format: yaml
  label: getziztu-com Meta API
  slug: getziztu-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-meta-api-openapi.yml
- filename: getziztu-com-music-api-openapi.yml
  format: yaml
  label: getziztu-com Music API
  slug: getziztu-com-music-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-music-api-openapi.yml
- filename: getziztu-com-places-api-openapi.yml
  format: yaml
  label: getziztu-com Places API
  slug: getziztu-com-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-places-api-openapi.yml
- filename: getziztu-com-projects-api-openapi.yml
  format: yaml
  label: getziztu-com Projects API
  slug: getziztu-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-projects-api-openapi.yml
- filename: getziztu-com-script-api-openapi.yml
  format: yaml
  label: getziztu-com Script API
  slug: getziztu-com-script-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-script-api-openapi.yml
- filename: getziztu-com-shots-api-openapi.yml
  format: yaml
  label: getziztu-com Shots API
  slug: getziztu-com-shots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-shots-api-openapi.yml
- filename: getziztu-com-tools-api-openapi.yml
  format: yaml
  label: getziztu-com Tools API
  slug: getziztu-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getziztu-com/openapi/getziztu-com-tools-api-openapi.yml
consequence_counts:
  physical: 1
  read: 16
  safety-critical: 1
  write: 38
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Getziztu Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /tools/{tool}/runs/{pid}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /tools/{tool}/runs/{pid}/message
operation_count: 56
overview: 'getziztu-com exposes 56 API operations that an AI agent could call, of which 40 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 38 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: getziztu-com
provider_slug: getziztu-com
slug: getziztu-com-agentic-access
source_filename: getziztu-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/getziztu-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 56\n  by_action_class:\n    connected: 16\n    acting: 40\n  by_consequence:\n    read: 16\n    write: 38\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /openapi.json\n  method: get\n  operationId: getOpenApiSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{pid}\n  method: patch\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/characters\n  method: post\n  operationId: createCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/characters/{cid}\n  method: patch\n  operationId: updateCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/characters/{cid}\n\
  \  method: delete\n  operationId: deleteCharacter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/places\n  method: post\n  operationId: createPlace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/places/{lid}\n  method: patch\n  operationId: updatePlace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /projects/{pid}/places/{lid}\n  method: delete\n  operationId: deletePlace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/shots\n  method: get\n  operationId: listShots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{pid}/shots\n  method: post\n  operationId: createShot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/shots/{sid}\n\
  \  method: patch\n  operationId: updateShot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/shots/{sid}\n  method: delete\n  operationId: deleteShot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/music\n  method: get\n  operationId: listMusic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{pid}/music\n  method: post\n  operationId: createMusic\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/music/{mid}\n  method: patch\n  operationId: updateMusic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/music/{mid}\n  method: delete\n  operationId: deleteMusic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/director/plan\n \
  \ method: post\n  operationId: directorPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/director/chat\n  method: post\n  operationId: directorChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/generate/frames\n  method: post\n  operationId: generateFrames\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /projects/{pid}/generate/animate\n  method: post\n  operationId: generateAnimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/generate/music\n  method: post\n  operationId: generateMusicPaid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/generate/character-images\n  method: post\n  operationId: generateCharacterImages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/generate/place-plates\n  method: post\n  operationId: generatePlacePlates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/generate/director-action\n  method: post\n  operationId: generateDirectorAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/quote\n  method: post\n  operationId: quoteOp\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/export\n  method: post\n  operationId: exportFilm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/export/plan\n  method: get\n  operationId: exportPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{pid}/media/{aid}/file\n  method: get\n  operationId: downloadMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jid}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jid}/cancel\n  method: post\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/script\n  method: get\n  operationId: readScript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /script/draft\n  method: post\n  operationId: startScriptDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/script/jobs/{jid}\n  method: get\n  operationId: getScriptJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{pid}/script/ask\n  method: post\n  operationId: askScriptEditor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/script/edits\n\
  \  method: post\n  operationId: decideScriptEdits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/script/doctor\n  method: post\n  operationId: runScriptDoctor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/script/versions\n  method: get\n  operationId: listScriptVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{pid}/script/versions/{vid}/restore\n  method: post\n\
  \  operationId: restoreScriptVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /script/import\n  method: post\n  operationId: importScript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{pid}/script/export\n  method: post\n  operationId: exportScript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /projects/{pid}/script/shots\n  method: post\n  operationId: scriptToShots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools\n  method: get\n  operationId: listToolsCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/recommend\n  method: post\n  operationId: recommendTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/{tool}/runs\n  method: get\n  operationId: listRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/{tool}/runs\n  method: post\n  operationId: startRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/{tool}/runs/{pid}\n  method: get\n  operationId: getRunStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/{tool}/runs/{pid}/approve\n  method: post\n  operationId:\
  \ approveRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/{tool}/runs/{pid}/stop\n  method: post\n  operationId: stopRun\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tools/{tool}/runs/{pid}/message\n  method: post\n  operationId: messageRun\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/{tool}/quote\n  method: post\n  operationId: quoteRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/getziztu-com/agentic-access/getziztu-com-agentic-access.yml
summary_line: 56 operations · 40 acting · 1 human-in-the-loop
tags:
- Company
- AI
- Video
- SocialMedia
- ContentCreation
---
