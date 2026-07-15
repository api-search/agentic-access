---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 8
api_specs:
- filename: predictive-oncology-model-and-data-clearinghouse-openapi.json
  format: json
  label: MoDaC REST API
  slug: modac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predictive-oncology-model-and-data-clearinghouse/refs/heads/main/openapi/predictive-oncology-model-and-data-clearinghouse-openapi.json
consequence_counts:
  read: 8
  safety-critical: 29
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 29
kind: agentic-access
layout: agentic-access
method: generated
name: Predictive Oncology Model And Data Clearinghouse Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /addCollection
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /addDatafile
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /addbulk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/collection/**
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/collection/query
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/dataObject/**/generateDownloadRequestURL
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/dataObject/**/syncDownload
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/dataObject/query
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/model/evaluate/**
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/models/evaluate/**
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/collection/**/download
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/dataObject/**
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/dataObject/**/download
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/download
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/registration
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /collection
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /delete/datafile
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /deleteCollection
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /deletePredictions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /download
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /downloadfiles/download
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /downloadsync
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /downloadtask
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /emailNotifications/subscribe
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /metaDataPermissionsList
operation_count: 37
overview: 'Predictive Oncology Model and Data Clearinghouse exposes 37 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 29 safety-critical.


  29 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Predictive Oncology Model and Data Clearinghouse
provider_slug: predictive-oncology-model-and-data-clearinghouse
slug: predictive-oncology-model-and-data-clearinghouse-agentic-access
source_filename: predictive-oncology-model-and-data-clearinghouse-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/predictive-oncology-model-and-data-clearinghouse-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    acting: 29\n    connected: 8\n  by_consequence:\n    safety-critical: 29\n    read: 8\n  human_in_the_loop_required: 29\noperations:\n- path: /api/v2/registration\n  method: put\n  operationId: bulkRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/dataObject/**\n\
  \  method: get\n  operationId: getDataObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/dataObject/**\n  method: put\n  operationId: registerDataObject\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/collection/**\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/collection/**\n  method: put\n  operationId: registerCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /uploadtask\n  method: post\n  operationId: retryUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /predictionAccessGroups\n  method: post\n  operationId: savePredictionAccessGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /performInferencing\n\
  \  method: post\n  operationId: performInfer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /performInferencing/performModelAnalysis\n  method: post\n  operationId: performModelAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /metaDataPermissionsList\n  method: post\n  operationId: savePermissionsList\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /emailNotifications/subscribe\n  method: post\n  operationId: sendEmailUpdates\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /downloadtask\n  method: post\n  operationId: retryDownload\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /downloadsync\n  method: post\n\
  \  operationId: download\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /downloadfiles/download\n  method: post\n  operationId: download_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /download\n  method: post\n  operationId: download_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /deletePredictions\n  method: post\n  operationId: deletePredictions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /deleteCollection\n  method: post\n  operationId: deletCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /delete/datafile\n  method: post\n  operationId: deleteObject\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /collection\n  method: post\n  operationId: updateCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/download\n  method: post\n  operationId: downloadDataObjectsOrCollections\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/v2/dataObject/**/download\n  method: post\n  operationId: syncAndasynchronousDownload\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/collection/**/download\n  method: post\n  operationId: collectionDownload\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/models/evaluate/**\n  method: post\n  operationId: performModelEvaluationForReferenceDatasets\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/model/evaluate/**\n  method: get\n  operationId: getStatusByTaskId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/model/evaluate/**\n  method: post\n  operationId: performModelEvaluationForDatasets\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/dataObject/query\n  method: post\n  operationId: queryDataObjects\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/dataObject/**/syncDownload\n  method: post\n  operationId: synchronousDownload\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/dataObject/**/generateDownloadRequestURL\n  method: post\n  operationId: generateDownloadRequestURL\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/collection/query\n  method: post\n  operationId: queryCollections\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /addbulk\n  method: post\n  operationId: createDatafile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /addDatafile\n  method: post\n  operationId: createDatafile_1\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /addCollection\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/registration/**\n  method: get\n  operationId: getDataObjectsRegistrationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/download/**\n  method: get\n  operationId: getDataObjectsOrCollectionsDownloadStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dataObject/download/**\n  method: get\n  operationId: getDataObjectDownloadStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/collection/download/**\n  method: get\n  operationId: getCollectionDownloadStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/authenticate\n  method: get\n  operationId: authenticate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predictive-oncology-model-and-data-clearinghouse/refs/heads/main/agentic-access/predictive-oncology-model-and-data-clearinghouse-agentic-access.yml
summary_line: 37 operations · 29 acting · 29 human-in-the-loop
tags:
- Cancer Research
- Clinical Data
- Datasets
- Machine Learning
- Oncology
---
