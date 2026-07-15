---
acting_count: 1250
action_class_counts:
  acting: 1250
api_specs:
- filename: ovp.openapi.json
  format: json
  label: Kaltura VPaaS API
  slug: vpaas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kaltura/developer-platform/master/ovp.openapi.json
- filename: ott.openapi.json
  format: json
  label: Kaltura OTT Backend API
  slug: ott-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/kaltura/developer-platform/master/ott.openapi.json
consequence_counts:
  physical: 41
  safety-critical: 41
  write: 1168
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 41
kind: agentic-access
layout: agentic-access
method: generated
name: Kaltura Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/accesscontrol/action/add
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/accesscontrol/action/delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/accesscontrol/action/get
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/accesscontrol/action/list
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/accesscontrol/action/update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/accesscontrolprofile/action/add
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/accesscontrolprofile/action/delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/accesscontrolprofile/action/get
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/accesscontrolprofile/action/list
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/accesscontrolprofile/action/update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/adminuser/action/resetPassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batch/action/resetJobExecutionAttempts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/configLoaded
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/getCommand
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/getFullStatus
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/getOrCreateScheduler
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/kill
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/listCommands
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/listSchedulers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/listWorkers
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/reportStatus
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/setCommandResult
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/setSchedulerConfig
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/setWorkerConfig
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /service/batchcontrol/action/startWorker
operation_count: 1250
overview: 'Kaltura exposes 1250 API operations that an AI agent could call, of which 1250 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1168 write, 41 physical, and 41 safety-critical.


  41 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kaltura
provider_slug: kaltura
slug: kaltura-agentic-access
source_filename: kaltura-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ott.openapi.json, openapi/ovp.openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1250\n  by_action_class:\n    acting: 1250\n  by_consequence:\n    write: 1168\n    physical: 41\n    safety-critical: 41\n  human_in_the_loop_required: 41\noperations:\n- path: /service/announcement/action/add\n  method: post\n  operationId: announcement.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/announcement/action/delete\n  method: post\n\
  \  operationId: announcement.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/announcement/action/enableSystemAnnouncements\n  method: post\n  operationId: announcement.enableSystemAnnouncements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/announcement/action/list\n  method: post\n  operationId: announcement.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/announcement/action/update\n  method: post\n  operationId: announcement.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/announcement/action/updateStatus\n  method: post\n  operationId: announcement.updateStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/apptoken/action/add\n  method: post\n  operationId: appToken.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/apptoken/action/delete\n  method: post\n  operationId: appToken.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/apptoken/action/get\n  method: post\n  operationId: appToken.get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/apptoken/action/startSession\n  method: post\n  operationId:\
  \ appToken.startSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/asset/action/add\n  method: post\n  operationId: asset.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/asset/action/count\n  method: post\n  operationId: asset.count\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /service/asset/action/delete\n  method: post\n  operationId: asset.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/asset/action/get\n  method: post\n  operationId: asset.get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/asset/action/getAdsContext\n  method: post\n  operationId: asset.getAdsContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/asset/action/getPlaybackContext\n  method: post\n  operationId: asset.getPlaybackContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/asset/action/list\n  method: post\n  operationId: asset.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/asset/action/removeMetasAndTags\n  method: post\n  operationId: asset.removeMetasAndTags\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/asset/action/update\n  method: post\n  operationId: asset.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/assetcomment/action/add\n  method: post\n  operationId: assetComment.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/assetcomment/action/list\n  method: post\n\
  \  operationId: assetComment.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/assetfile/action/getContext\n  method: post\n  operationId: assetFile.getContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/assetfile/action/playManifest\n  method: post\n  operationId: assetFile.playManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /service/assethistory/action/clean\n  method: post\n  operationId: assetHistory.clean\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/assethistory/action/list\n  method: post\n  operationId: assetHistory.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/assetstatistics/action/query\n  method: post\n  operationId: assetStatistics.query\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/assetstruct/action/add\n  method: post\n  operationId: assetStruct.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/assetstruct/action/delete\n  method: post\n  operationId: assetStruct.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/assetstruct/action/list\n  method: post\n  operationId: assetStruct.list\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/assetstruct/action/update\n  method: post\n  operationId: assetStruct.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/bookmark/action/add\n  method: post\n  operationId: bookmark.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /service/bookmark/action/list\n  method: post\n  operationId: bookmark.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdnadapterprofile/action/add\n  method: post\n  operationId: cdnAdapterProfile.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdnadapterprofile/action/delete\n  method: post\n  operationId: cdnAdapterProfile.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdnadapterprofile/action/generateSharedSecret\n  method: post\n  operationId: cdnAdapterProfile.generateSharedSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdnadapterprofile/action/list\n  method: post\n  operationId: cdnAdapterProfile.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdnadapterprofile/action/update\n  method: post\n  operationId:\
  \ cdnAdapterProfile.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdnpartnersettings/action/get\n  method: post\n  operationId: cdnPartnerSettings.get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdnpartnersettings/action/update\n  method: post\n  operationId: cdnPartnerSettings.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdvradapterprofile/action/add\n  method: post\n  operationId: cDVRAdapterProfile.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdvradapterprofile/action/delete\n  method: post\n  operationId: cDVRAdapterProfile.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdvradapterprofile/action/generateSharedSecret\n  method: post\n  operationId: cDVRAdapterProfile.generateSharedSecret\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdvradapterprofile/action/list\n  method: post\n  operationId: cDVRAdapterProfile.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/cdvradapterprofile/action/update\n  method: post\n  operationId: cDVRAdapterProfile.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /service/channel/action/add\n  method: post\n  operationId: channel.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/channel/action/delete\n  method: post\n  operationId: channel.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/channel/action/get\n  method: post\n  operationId: channel.get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/channel/action/list\n  method: post\n  operationId: channel.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/channel/action/update\n  method: post\n  operationId: channel.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/collection/action/list\n  method: post\n  operationId: collection.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/compensation/action/add\n  method: post\n  operationId: compensation.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/compensation/action/delete\n  method: post\n  operationId: compensation.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/compensation/action/get\n  method: post\n  operationId: compensation.get\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgroup/action/add\n  method: post\n  operationId: configurationGroup.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgroup/action/delete\n  method: post\n  operationId: configurationGroup.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /service/configurationgroup/action/get\n  method: post\n  operationId: configurationGroup.get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgroup/action/list\n  method: post\n  operationId: configurationGroup.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgroup/action/update\n  method: post\n  operationId: configurationGroup.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgroupdevice/action/add\n  method: post\n  operationId: configurationGroupDevice.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgroupdevice/action/delete\n  method: post\n  operationId: configurationGroupDevice.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgroupdevice/action/get\n\
  \  method: post\n  operationId: configurationGroupDevice.get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgroupdevice/action/list\n  method: post\n  operationId: configurationGroupDevice.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgrouptag/action/add\n  method: post\n  operationId: configurationGroupTag.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgrouptag/action/delete\n  method: post\n  operationId: configurationGroupTag.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgrouptag/action/get\n  method: post\n  operationId: configurationGroupTag.get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurationgrouptag/action/list\n  method: post\n  operationId: configurationGroupTag.list\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurations/action/add\n  method: post\n  operationId: configurations.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurations/action/delete\n  method: post\n  operationId: configurations.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /service/configurations/action/get\n  method: post\n  operationId: configurations.get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurations/action/list\n  method: post\n  operationId: configurations.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurations/action/serveByDevice\n  method: post\n  operationId: configurations.serveByDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/configurations/action/update\n  method: post\n  operationId: configurations.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/country/action/list\n  method: post\n  operationId: country.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/coupon/action/get\n  method: post\n  operationId: coupon.get\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/currency/action/list\n  method: post\n  operationId: currency.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/devicebrand/action/list\n  method: post\n  operationId: deviceBrand.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/devicefamily/action/list\n\
  \  method: post\n  operationId: deviceFamily.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/drmprofile/action/list\n  method: post\n  operationId: drmProfile.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/email/action/send\n  method: post\n  operationId: email.send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/engagement/action/add\n  method: post\n  operationId: engagement.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/engagement/action/delete\n  method: post\n  operationId: engagement.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/engagement/action/get\n  method: post\n  operationId: engagement.get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/engagement/action/list\n  method: post\n  operationId: engagement.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/engagementadapter/action/add\n  method: post\n  operationId: engagementAdapter.add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/engagementadapter/action/delete\n  method: post\n  operationId:\
  \ engagementAdapter.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/engagementadapter/action/generateSharedSecret\n  method: post\n  operationId: engagementAdapter.generateSharedSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/engagementadapter/action/get\n  method: post\n  operationId: engagementAdapter.get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/engagementadapter/action/list\n  method: post\n  operationId: engagementAdapter.list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/engagementadapter/action/update\n  method: post\n  operationId: engagementAdapter.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service/entitlement/action/cancel\n  method: post\n  operationId: entitlement.cancel\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audie\n\n# --- truncated at 32 KB (450 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/kaltura/refs/heads/main/agentic-access/kaltura-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaltura/refs/heads/main/agentic-access/kaltura-agentic-access.yml
summary_line: 1250 operations · 1250 acting · 41 human-in-the-loop
tags:
- Video
- Live Streaming
- Transcoding
- Media Management
- Player
- Analytics
- Virtual Classroom
- OTT
- Open Source
---
