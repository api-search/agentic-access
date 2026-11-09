---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 21
api_specs:
- filename: fabrica-land-change-of-ownership-api-openapi.yml
  format: yaml
  label: fabrica-land Change Of Ownership API
  slug: fabrica-land-change-of-ownership-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-change-of-ownership-api-openapi.yml
- filename: fabrica-land-document-api-openapi.yml
  format: yaml
  label: fabrica-land Document API
  slug: fabrica-land-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-document-api-openapi.yml
- filename: fabrica-land-media-api-openapi.yml
  format: yaml
  label: fabrica-land Media API
  slug: fabrica-land-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-media-api-openapi.yml
- filename: fabrica-land-metadata-api-openapi.yml
  format: yaml
  label: fabrica-land Metadata API
  slug: fabrica-land-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-metadata-api-openapi.yml
- filename: fabrica-land-off-ramp-api-openapi.yml
  format: yaml
  label: fabrica-land Off Ramp API
  slug: fabrica-land-off-ramp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-off-ramp-api-openapi.yml
- filename: fabrica-land-on-ramp-api-openapi.yml
  format: yaml
  label: fabrica-land On Ramp API
  slug: fabrica-land-on-ramp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-on-ramp-api-openapi.yml
- filename: fabrica-land-pool-lending-api-openapi.yml
  format: yaml
  label: fabrica-land Pool Lending API
  slug: fabrica-land-pool-lending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-pool-lending-api-openapi.yml
- filename: fabrica-land-proof-of-ownership-api-openapi.yml
  format: yaml
  label: fabrica-land Proof Of Ownership API
  slug: fabrica-land-proof-of-ownership-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-proof-of-ownership-api-openapi.yml
- filename: fabrica-land-regrid-api-openapi.yml
  format: yaml
  label: fabrica-land Regrid API
  slug: fabrica-land-regrid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-regrid-api-openapi.yml
- filename: fabrica-land-syndication-api-openapi.yml
  format: yaml
  label: fabrica-land Syndication API
  slug: fabrica-land-syndication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-syndication-api-openapi.yml
- filename: fabrica-land-terrain-project-api-openapi.yml
  format: yaml
  label: fabrica-land Terrain Project API
  slug: fabrica-land-terrain-project-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-terrain-project-api-openapi.yml
- filename: fabrica-land-token-api-openapi.yml
  format: yaml
  label: fabrica-land Token API
  slug: fabrica-land-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-token-api-openapi.yml
- filename: fabrica-land-valuation-api-openapi.yml
  format: yaml
  label: fabrica-land Valuation API
  slug: fabrica-land-valuation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-valuation-api-openapi.yml
consequence_counts:
  physical: 2
  read: 21
  safety-critical: 2
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Fabrica Land Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /change-of-ownership/{workflowId}/user-info/{owner}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /document/md/convert/pdf
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /proof-of-ownership/{networkName}/{contractAddress}/{tokenId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /proof-of-ownership/{networkName}/{contractAddress}/{tokenId}
operation_count: 37
overview: 'fabrica-land exposes 37 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 12 write, 2 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: fabrica-land
provider_slug: fabrica-land
slug: fabrica-land-agentic-access
source_filename: fabrica-land-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/fabrica-land-v3-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    acting: 16\n    connected: 21\n  by_consequence:\n    safety-critical: 2\n    read: 21\n    write: 12\n    physical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /change-of-ownership/{workflowId}/user-info/{owner}\n  method: post\n  operationId: ChangeOfOwnershipController_SaveCollectedFieldsForChangeOfOwnership\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /document/md/convert/pdf\n  method: get\n  operationId: DocumentController_convertMarkdownToPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document/md/convert/pdf\n  method: post\n  operationId: DocumentController_convertMarkdownContentToPdfContent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /off-ramp/{networkName}/{contractAddress}\n  method: get\n  operationId: getOffRamps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /off-ramp/{networkName}/{contractAddress}/{tokenId}\n\
  \  method: get\n  operationId: getOffRamp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /off-ramp/{networkName}/{contractAddress}/{tokenId}\n  method: delete\n  operationId: cancelOffRamp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /off-ramp/{networkName}/{contractAddress}/{tokenId}/steps-and-fields\n  method: get\n  operationId: getStepsAndFieldsForOffRamp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /on-ramp/steps-and-fields/{country}/{admin}/{property}\n  method: get\n  operationId: getStepsAndFieldsForOnRamp\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /on-ramp/{networkName}/{contractAddress}\n  method: post\n  operationId: onRampProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-ramp/{networkName}/{contractAddress}\n  method: get\n  operationId: getOnRamps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /on-ramp/{networkName}/{contractAddress}/{tokenId}\n  method: get\n  operationId: getOnRamp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /on-ramp/{networkName}/{contractAddress}/{tokenId}\n\
  \  method: delete\n  operationId: cancelOnRamp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-ramp/{networkName}/{contractAddress}/{tokenId}\n  method: patch\n  operationId: patchOnRamp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-ramp/{networkName}/{contractAddress}/{tokenId}/claim\n  method: post\n  operationId: claimOnRampPremint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-ramp/{networkName}/{contractAddress}/{tokenId}/claim-session\n  method: post\n  operationId: issueOnRampClaimSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-ramp/{networkName}/{contractAddress}/{tokenId}/configuration\n  method: put\n  operationId: updateOnRampConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-ramp/{networkName}/{contractAddress}/{tokenId}/configuration\n  method: patch\n  operationId:\
  \ patchOnRampConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /on-ramp/{networkName}/{contractAddress}/{tokenId}/mark-celebration-complete\n  method: post\n  operationId: markOnRampCelebrationComplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pdf417\n  method: get\n  operationId: generatePdf417Barcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pool-lending/{networkName}/{contractAddress}/oracle-report\n\
  \  method: get\n  operationId: getPoolLendingOracleReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pool-lending/{networkName}/{poolAddress}/{contractAddress}/{tokenId}/signed-valuation\n  method: get\n  operationId: getPoolLendingValuation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /proof-of-ownership/{networkName}/{contractAddress}/{tokenId}\n  method: post\n  operationId: proveOwnershipOfProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /proof-of-ownership/{networkName}/{contractAddress}/{tokenId}\n\
  \  method: get\n  operationId: getProofOfOwnership\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /proof-of-ownership/{networkName}/{contractAddress}/{tokenId}\n  method: delete\n  operationId: cancelProofOfOwnership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /proof-of-ownership/{networkName}/{contractAddress}/{tokenId}/steps-and-fields\n  method: get\n  operationId: getStepsAndFieldsForProofOfOwnership\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /regrid/tile/{z}/{x}/{y}\n  method:\
  \ get\n  operationId: getRegridTile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /syndication/{networkName}/{contractAddress}/rets\n  method: get\n  operationId: retsFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /terrain-project/listing/{networkName}\n  method: post\n  operationId: syncTerrainProjectListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terrain-project/listing/{networkName}/{vendorId}\n  method: delete\n  operationId: cancelTerrainProjectListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token/{networkName}/{contractAddress}/token/{tokenId}/configuration\n  method: patch\n  operationId: patchTokenConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token/{networkName}/{contractAddress}/{tokenId}/title-docs\n  method: get\n  operationId: getTitleDocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token/{networkName}/{contractAddress}/{tokenId}/valuation-report\n  method: get\n  operationId: getValuationReport\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valuation/v1/{networkName}/{contractAddress}/{tokenId}\n  method: get\n  operationId: getValuation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{networkName}/{contractAddress}/collection/image\n  method: get\n  operationId: getCollectionImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{networkName}/{contractAddress}/{tokenIdOrWalletAddress}/image\n  method: get\n  operationId: getImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{networkName}/{contractAddress}/{tokenId}\n  method: get\n  operationId: getMetadata\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{networkName}/{contractAddress}/{tokenId}/animation\n  method: get\n  operationId: getAnimationHtml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/fabrica-land/agentic-access/fabrica-land-agentic-access.yml
summary_line: 37 operations · 16 acting · 2 human-in-the-loop
tags:
- Company
- Real Estate
- Blockchain
- Marketplace
- Fintech
---
