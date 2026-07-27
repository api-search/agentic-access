---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 35
api_specs:
- filename: sk-telecom-ax-tts-openapi.json
  format: json
  label: SK Telecom A.X TTS API
  slug: sk-telecom-ax-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-ax-tts-openapi.json
- filename: sk-telecom-facecan-openapi.json
  format: json
  label: SK Telecom A. facecan API
  slug: sk-telecom-facecan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-facecan-openapi.json
- filename: sk-telecom-puzzle-place-congestion-openapi.json
  format: json
  label: SK Telecom Puzzle Place Congestion API
  slug: sk-telecom-puzzle-place-congestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-puzzle-place-congestion-openapi.json
- filename: sk-telecom-puzzle-residence-openapi.json
  format: json
  label: SK Telecom Puzzle Residence API
  slug: sk-telecom-puzzle-residence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-puzzle-residence-openapi.json
- filename: sk-telecom-meta-openapi.json
  format: json
  label: SK Telecom META API
  slug: sk-telecom-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-meta-openapi.json
- filename: sk-telecom-ovs-openapi.json
  format: json
  label: SK Telecom OVS API
  slug: sk-telecom-ovs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/openapi/sk-telecom-ovs-openapi.json
consequence_counts:
  read: 35
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sk Telecom Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 55
overview: 'SK Telecom exposes 55 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read and 20 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SK Telecom
provider_slug: sk-telecom
slug: sk-telecom-agentic-access
source_filename: sk-telecom-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/sk-telecom-ax-tts-openapi.json, openapi/sk-telecom-facecan-openapi.json, openapi/sk-telecom-meta-openapi.json,\n  openapi/sk-telecom-ovs-openapi.json, openapi/sk-telecom-puzzle-place-congestion-openapi.json,\n  openapi/sk-telecom-puzzle-residence-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    connected: 35\n    acting: 20\n  by_consequence:\n    read: 35\n    write: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /voice\n  method: get\n  operationId: get-voices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tts\n  method: post\n\
  \  operationId: text-to-speech-tts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /segmentation\n  method: post\n  operationId: text-to-speech-with-timestamp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subject\n  method: post\n  operationId: subject-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/subject\n  method: get\n  operationId: subject-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subject/{subject_id}\n  method: delete\n  operationId: subject-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/group\n  method: get\n  operationId: group-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/group\n  method: post\n  operationId: group-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/group/{group_id}\n  method: delete\n  operationId: group-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/face\n  method: get\n  operationId: subject-list-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/face\n  method: post\n  operationId: face-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/face/{face_id}\n  method: delete\n  operationId: face-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recognize\n  method: post\n  operationId: face-recognize-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/detect\n  method: post\n  operationId: face-detect-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/landmark\n  method: post\n  operationId: face-landmark-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /golf/v1/create_analyzer\n  method: post\n  operationId: create_analyzer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /golf/v1/get_result/{JobID}\n  method: get\n  operationId: get_result\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /golf/v1/e2e\n  method: post\n  operationId: e2e\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lpr/v1\n  method: post\n  operationId: lpr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pose/v1/create_analyzer\n  method: post\n  operationId: create-analyzer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /pose/v1/get_result/{JobID}\n  method: get\n  operationId: start_analyzer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pose/v1/e2e\n  method: post\n  operationId: e2e-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v20/company/info/me\n  method: get\n  operationId: 내-회사-정보-조회\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v20/company/info/devices/{companyId}\n  method: get\n  operationId: 회사-전체-단말-리스트-조회\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /v20/company/info/{companyId}\n  method: get\n  operationId: 회사-정보-조회\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v20/company/info/devices/cnt/{companyId}\n  method: get\n  operationId: 회사-전체-단말-수-조회\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v20/device\n  method: post\n  operationId: 단말-등록\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v20/device/{serialNo}\n  method: get\n  operationId: 단말-정보-조회\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v20/device/{serialNo}\n  method: delete\n  operationId: 단말-삭제\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v20/statistics/device/event/{serialNo}\n  method: post\n  operationId: 단말별-메시지-전달\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v20/statistics/device/event/{serialNo}\n  method: get\n  operationId: 단말별-이벤트-통계\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v20/statistics/company/event/{companyId}\n  method: get\n  operationId: 회사별-이벤트-통계\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v20/message/company/{companyId}\n  method: post\n  operationId: 전체-단말-메시지-전달\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v20/statistics/event/raw\n  method: get\n  operationId: 이벤트-raw-data-정보-조회\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta/pois\n  method: get\n  operationId: pois\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta/areas\n  method: get\n  operationId: areas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /congestion/rltm/pois/{poiId}\n  method: get\n  operationId: poicongestionrltm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /congestion/stat/raw/hourly/pois/{poiId}\n  method: get\n  operationId: poicongestionraw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /congestion/stat/hourly/pois/{poiId}\n  method: get\n  operationId: poicongestionstat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /congestion/rltm/areas/{areaId}\n\
  \  method: get\n  operationId: areacongestionrltm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /congestion/stat/raw/hourly/areas/{areaId}\n  method: get\n  operationId: areacongestionraw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /congestion/stat/hourly/areas/{areaId}\n  method: get\n  operationId: areacongestionstat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visit/count/raw/daily/pois/{poiId}\n  method: get\n  operationId: poivisitcount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visit/distance/stat/daily/pois/{poiId}\n  method: get\n  operationId:\
  \ poivisitdistance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visit/seg/stat/daily/pois/{poiId}\n  method: get\n  operationId: poivisitseg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visit/count/raw/daily/areas/{areaId}\n  method: get\n  operationId: areavisitcount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visit/distance/stat/daily/areas/{areaId}\n  method: get\n  operationId: areavisitdistance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visit/seg/stat/daily/areas/{areaId}\n  method: get\n  operationId: areavisitseg\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visit/type/stat/daily/areas/{areaId}\n  method: get\n  operationId: areavisittype\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /biz-category/stat/monthly/areas/{areaId}\n  method: get\n  operationId: areabizcategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta/apts\n  method: get\n  operationId: apts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{category}/stat/monthly/apts/{kaptCode}\n  method: get\n  operationId: aptcategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /resident/subway-use-rate/stat/monthly/apts/{kaptCode}\n  method: get\n  operationId: aptsubwayuserate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resident/age/stat/monthly/apts/{kaptCode}\n  method: get\n  operationId: aptresidentage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resident/demo-feature/stat/monthly/apts/{kaptCode}\n  method: get\n  operationId: aptresidentdemo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sk-telecom/refs/heads/main/agentic-access/sk-telecom-agentic-access.yml
summary_line: 55 operations · 20 acting
tags:
- Telecommunications
- South Korea
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- 5G
- Identity Verification
- SIM Swap
- Artificial Intelligence
- Location
- Big Data
---
