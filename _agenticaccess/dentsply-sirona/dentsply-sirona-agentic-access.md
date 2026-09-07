---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 19
api_specs:
- filename: dentsply-sirona-intraoral-modality-openapi.yml
  format: yaml
  label: Dentsply Sirona Intraoral Imaging Modality API
  slug: dsio-modality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/openapi/dentsply-sirona-intraoral-modality-openapi.yml
- filename: dentsply-sirona-intraoral-filters-openapi.yml
  format: yaml
  label: Dentsply Sirona Intraoral Imaging Filters API
  slug: dsio-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/openapi/dentsply-sirona-intraoral-filters-openapi.yml
- filename: dentsply-sirona-intraoral-exposure-openapi.yml
  format: yaml
  label: Intraoral Exposure API
  slug: io-exposure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/openapi/dentsply-sirona-intraoral-exposure-openapi.yml
consequence_counts:
  read: 19
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dentsply Sirona Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Dentsply Sirona exposes 30 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dentsply Sirona
provider_slug: dentsply-sirona
slug: dentsply-sirona-agentic-access
source_filename: dentsply-sirona-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: generated\nsource: openapi/dentsply-sirona-intraoral-exposure-openapi.yml, openapi/dentsply-sirona-intraoral-filters-openapi.yml,\n  openapi/dentsply-sirona-intraoral-modality-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 19\n    acting: 11\n  by_consequence:\n    read: 19\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /generator\n  method: get\n  operationId: getAllGenerators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generator/{id}\n  method: get\n  operationId: getGenerator\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generator/{id}/exposure\n  method: get\n  operationId: getExposures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generator/{id}/exposure/{exposureId}\n  method: get\n  operationId: getExposure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images\n  method: post\n  operationId: createImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/modality\n  method: post\n  operationId: modalityImage\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/{id}\n  method: get\n  operationId: getImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/{id}\n  method: delete\n  operationId: deleteImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/{id}/media\n  method: get\n  operationId: getImageMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /images/{id}/filters/unmap\n  method: post\n  operationId: unmapImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/{id}/filters/select\n  method: post\n  operationId: filterSelect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/{id}/filters/supreme\n  method: post\n  operationId: filterSupreme\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/{id}/filters/ae\n  method: post\n  operationId: filterAE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices\n  method: get\n  operationId: getAllDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/subscribe\n  method: get\n  operationId: subscribeDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{deviceId}\n  method: get\n  operationId: getDeviceInfo\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{deviceId}/sensor\n  method: get\n  operationId: getSensorInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /acquisition\n  method: post\n  operationId: createAcquisitionSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acquisition\n  method: get\n  operationId: getSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /acquisition/{sessionId}\n  method: get\n  operationId: getAcquisitionSession\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /acquisition/{sessionId}\n  method: put\n  operationId: updateAcquisitionSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acquisition/{sessionId}\n  method: delete\n  operationId: deleteAcquisitionSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acquisition/{sessionId}/status\n  method: get\n  operationId: getAcquisitionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /acquisition/{sessionId}/status/subscribe\n  method: get\n  operationId: subscribeAcquisitionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /acquisition/{sessionId}/info\n  method: get\n  operationId: getAcquisitionInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /acquisition/{sessionId}/info\n  method: put\n  operationId: setAcquisitionInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acquisition/{sessionId}/images\n  method: get\n  operationId:\
  \ getImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /acquisition/{sessionId}/images/{imageId}\n  method: get\n  operationId: getImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /acquisition/{sessionId}/images/{imageId}/media\n  method: get\n  operationId: getImageMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /acquisition/{sessionId}/images/{imageId}/preview\n  method: get\n  operationId: getImagePreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/agentic-access/dentsply-sirona-agentic-access.yml
summary_line: 30 operations · 11 acting
tags:
- CAD/CAM
- CEREC
- Dental
- DS Core
- Imaging
- Intraoral Imaging
- Lab Management
- Medical Devices
- Practice Management
- Fortune 1000
---
