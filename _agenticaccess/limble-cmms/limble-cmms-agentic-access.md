---
acting_count: 293
action_class_counts:
  acting: 293
  connected: 119
api_specs:
- filename: limble-cmms-limble-api-v2-openapi.yml
  format: yaml
  label: Limble API V2
  slug: limble-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limble-cmms/refs/heads/main/openapi/limble-cmms-limble-api-v2-openapi.yml
- filename: limble-cmms-routes-api-openapi.yml
  format: yaml
  label: Limble CMMS Routes API
  slug: limble-cmms-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limble-cmms/refs/heads/main/openapi/limble-cmms-routes-api-openapi.yml
consequence_counts:
  physical: 26
  read: 119
  write: 267
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Limble Cmms Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/po
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/po
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/po/{poID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/po/{poID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/po/{poID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/po/{poID}/comments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/po/{poID}/comments/{commentID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/po/{poID}/comments/{commentID}/file
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/po/{poID}/comments/{commentID}/file
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/po/{poID}/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/po/{poID}/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/po/{poID}/items/{poItemID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/po/{poID}/items/{poItemID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/po/{poID}/items/{poItemID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/po/{poID}/items/{poItemID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/po/{poID}/state
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/tasks/{taskID}/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/tasks/{taskID}/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/tasks/{taskID}/invoices/{invoiceID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/tasks/{taskID}/invoices/{invoiceID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/tasks/{taskID}/invoices/{invoiceID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/tasks/{taskID}/invoices/{invoiceID}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/tasks/{taskID}/invoices/{invoiceID}/file
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/tasks/{taskID}/invoices/{invoiceID}/file
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/tasks/{taskID}/invoices/{invoiceID}/file
operation_count: 412
overview: 'Limble CMMS exposes 412 API operations that an AI agent could call, of which 293 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 119 read, 267 write, and 26 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Limble CMMS
provider_slug: limble-cmms
slug: limble-cmms-agentic-access
source_filename: limble-cmms-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: generated\nsource: openapi/limble-cmms-limble-api-v2-openapi.yml, openapi/limble-cmms-routes-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 412\n  by_action_class:\n    connected: 119\n    acting: 293\n  by_consequence:\n    read: 119\n    write: 267\n    physical: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/{assetID}/image\n  method: put\n  operationId: putAssetsByAssetIDImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/{assetID}/image\n  method: delete\n  operationId: deleteAssetsByAssetIDImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/fields\n  method: get\n  operationId: getAssetsFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/fields\n  method: post\n  operationId: postAssetsFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/fields/suggested\n  method: get\n  operationId: getAssetsFieldsSuggested\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/fields/history\n  method: get\n  operationId: getAssetsFieldsHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/{assetID}/fields\n  method: put\n  operationId: putAssetsByAssetIDFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/fields/{valueID}\n\
  \  method: delete\n  operationId: deleteAssetsFieldsByValueID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/fields/{valueID}\n  method: patch\n  operationId: patchAssetsFieldsByValueID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/logs/file/{fileID}\n  method: delete\n  operationId: deleteAssetsLogsFileByFileID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/{assetID}/logs/{logID}/file\n  method: put\n  operationId: putAssetsByAssetIDLogsByLogIDFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/{assetID}/logs\n  method: get\n  operationId: getAssetsByAssetIDLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/{assetID}/logs\n  method: post\n  operationId: postAssetsByAssetIDLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/logs/{logID}\n  method: patch\n  operationId: patchAssetsLogsByLogID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/logs/{logID}\n  method: delete\n  operationId: deleteAssetsLogsByLogID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/fields/{fieldID}/options\n  method: get\n  operationId: getAssetsFieldOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/fields/{fieldID}/options\n  method: post\n  operationId: postAssetsFieldOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/fields/{fieldID}/options\n  method: put\n  operationId: putAssetsFieldOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/fields/{fieldID}/options/{optionName}\n  method: delete\n  operationId: deleteAssetsFieldOption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/fields/batch/update\n  method: post\n  operationId: postAssetsFieldsBatchUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/parts\n  method: get\n  operationId: getAssetsParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets\n  method: get\n  operationId: getAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/assets\n  method: post\n  operationId: postAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/{assetID}\n  method: delete\n  operationId: deleteAssetsByAssetID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/{assetID}\n  method: patch\n  operationId: patchAssetsByAssetID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/{assetID}/move\n  method: patch\n  operationId: patchAssetsByAssetIDMove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/locations\n  method: post\n  operationId: postLocations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/locations\n  method: get\n  operationId: getLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/locations/{locationID}\n\
  \  method: patch\n  operationId: patchLocationsByLocationID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/locations/{locationID}\n  method: delete\n  operationId: deleteLocationsByLocationID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/{partID}/image\n  method: put\n  operationId: putPartsByPartIDImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/{partID}/image\n  method: delete\n  operationId: deletePartsByPartIDImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/categories\n  method: post\n  operationId: postPartsCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/categories\n  method: get\n  operationId: getPartsCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /v2/parts/categories/{categoryID}\n  method: patch\n  operationId: patchPartsCategoriesByCategoryID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/categories/{categoryID}\n  method: delete\n  operationId: deletePartsCategoriesByCategoryID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/fields\n  method: get\n  operationId: getPartsFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/parts/fields\n  method: post\n  operationId: postPartsFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/fields/suggested\n  method: get\n  operationId: getPartsFieldsSuggested\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/fields/{valueID}\n  method: patch\n  operationId: patchPartsFieldsByValueID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/fields/{valueID}\n\
  \  method: delete\n  operationId: deletePartsFieldsByValueID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/{partID}/fields\n  method: put\n  operationId: putPartsByPartIDFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/{partID}/logs\n  method: get\n  operationId: getPartsByPartIDLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/{partID}/logs\n  method: post\n  operationId:\
  \ postPartsByPartIDLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/logs/{logID}\n  method: patch\n  operationId: patchPartsLogsByLogID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/logs/{logID}\n  method: delete\n  operationId: deletePartsLogsByLogID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/parts/logs\n  method: get\n  operationId: getPartsLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/{partID}/purchasables\n  method: get\n  operationId: getPartsByPartIDPurchasables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/vendors/associations\n  method: get\n  operationId: getPartsVendorsAssociations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/vendors/associations\n  method: post\n  operationId: postPartsVendorsAssociations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/vendors/associations/{relationID}\n  method: delete\n  operationId: deletePartsVendorsAssociationsByRelationID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts\n  method: get\n  operationId: getParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts\n  method: post\n  operationId: postParts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/parts/fields/{fieldID}/options\n  method: get\n  operationId: getPartsFieldOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/fields/{fieldID}/options\n  method: post\n  operationId: postPartsFieldOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/fields/{fieldID}/options\n  method: put\n  operationId: putPartsFieldOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/parts/fields/{fieldID}/options/{optionName}\n  method: delete\n  operationId: deletePartsFieldOption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/{partID}\n  method: patch\n  operationId: patchPartsByPartID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/{partID}\n  method: delete\n  operationId: deletePartsByPartID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/usage\n  method: get\n  operationId: getPartsUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/{taskID}/invoices/{invoiceID}/file\n  method: put\n  operationId: putTasksByTaskIDInvoicesByInvoiceIDFile\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskID}/invoices/{invoiceID}/file\n  method: delete\n  operationId: deleteTasksByTaskIDInvoicesByInvoiceIDFile\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/invoices\n  method: get\n  operationId: getTasksInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/{taskID}/invoices\n  method: put\n  operationId: putTasksByTaskIDInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskID}/invoices/{invoiceID}\n  method: delete\n  operationId: deleteTasksByTaskIDInvoicesByInvoiceID\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskID}/invoices/{invoiceID}\n  method: patch\n  operationId: patchTasksByTaskIDInvoicesByInvoiceID\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskID}/instructions/{instructionID}/options\n  method: get\n  operationId: getTasksByTaskIDInstructionsByInstructionIDOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/{taskID}/instructions/{instructionID}/options\n  method: post\n  operationId: postTasksByTaskIDInstructionsByInstructionIDOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/instructions/{instructionID}/options/{instructionOptionID}\n  method: delete\n  operationId: deleteTasksInstructionsByInstructionIDOptionsByInstructionOptionID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/instructions/{instructionID}/options/{instructionOptionID}\n\
  \  method: patch\n  operationId: patchTasksInstructionsByInstructionIDOptionsByInstructionOptionID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskID}/instructions\n  method: get\n  operationId: getTasksByTaskIDInstructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/{taskID}/instructions\n  method: post\n  operationId: postTasksByTaskIDInstructions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/tasks/instructions/{instructionID}\n  method: patch\n  operationId: patchTasksInstructionsByInstructionID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/instructions/{instructionID}\n  method: delete\n  operationId: deleteTasksInstructionsByInstructionID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/instructions/{instructionID}\n  method: get\n  operationId: getTasksInstructionsByInstructionID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/instructions\n  method: get\n  operationId: getTasksInstructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/instructions/{instructionID}/image\n  method: put\n  operationId: putTasksInstructionsByInstructionIDImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/instructions/{instructionID}/image\n  method: delete\n  operationId: deleteTasksInstructionsByInstructionIDImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskID}/image\n  method: put\n  operationId: putTasksByTaskIDImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskID}/image\n  method: delete\n  operationId: deleteTasksByTaskIDImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/labor\n  method: get\n  operationId: getTasksLabor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/labor/categories\n  method: get\n  operationId: getTasksLaborCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/{taskID}/parts\n  method: get\n  operationId: getTasksByTaskIDParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/{taskID}/parts\n  method: put\n  operationId: putTasksByTaskIDParts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/parts\n  method: get\n  operationId: getTasksParts\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/{taskID}/{partID}\n  method: delete\n  operationId: deleteTasksByTaskIDByPartID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskID}/comments\n  method: get\n  operationId: getTasksByTaskIDComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/{taskID}/comments\n  method: post\n  operationId: postTasksByTaskIDComments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskID}/tags\n  method: get\n  operationId: getTasksByTaskIDTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/{taskID}/tags\n  method: put\n  operationId: putTasksByTaskIDTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskID}/tags/{tagRaw}\n  method: delete\n  operationId: deleteTasksByTaskIDTagsByTagRaw\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /v2/work-requests/work-request-submissions\n  method: get\n  operationId: getWorkRequestsWorkRequestSubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/work-requests/work-request-submissions\n  method: post\n  operationId: postWorkRequestsWorkRequestSubmissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-requests/work-request-submissions/{workRequestSubmissionID}/approve\n  method: post\n  operationId: postWorkRequestSubmissionsApprove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-requests/work-request-submissions/{workRequestSubmissionID}/decline\n  method: post\n  operationId: postWorkRequestSubmissionsDecline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks\n  method: post\n  operationId: postTasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks\n  method: get\n  operationId: getTasks\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tasks/{taskID}\n  method: patch\n  operationId: patchTasksByTaskID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskID}\n  method: delete\n  operationId: deleteTasksByTaskID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (129 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/limble-cmms/refs/heads/main/agentic-access/limble-cmms-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limble-cmms/refs/heads/main/agentic-access/limble-cmms-agentic-access.yml
summary_line: 412 operations · 293 acting
tags:
- CMMS
- Maintenance Management
- Asset Management
- Manufacturing
- Facility Management
- Work Orders
---
