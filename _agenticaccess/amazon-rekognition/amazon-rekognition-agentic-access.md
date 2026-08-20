---
acting_count: 15
action_class_counts:
  acting: 15
api_specs:
- filename: amazon-rekognition-celebrity-recognition-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Celebrity Recognition API
  slug: amazon-rekognition-celebrity-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-celebrity-recognition-api-openapi.yml
- filename: amazon-rekognition-content-moderation-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Content Moderation API
  slug: amazon-rekognition-content-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-content-moderation-api-openapi.yml
- filename: amazon-rekognition-custom-labels-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Custom Labels API
  slug: amazon-rekognition-custom-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-custom-labels-api-openapi.yml
- filename: amazon-rekognition-face-collections-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Face Collections API
  slug: amazon-rekognition-face-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-face-collections-api-openapi.yml
- filename: amazon-rekognition-face-liveness-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Face Liveness API
  slug: amazon-rekognition-face-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-face-liveness-api-openapi.yml
- filename: amazon-rekognition-face-search-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Face Search API
  slug: amazon-rekognition-face-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-face-search-api-openapi.yml
- filename: amazon-rekognition-facial-analysis-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Facial Analysis API
  slug: amazon-rekognition-facial-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-facial-analysis-api-openapi.yml
- filename: amazon-rekognition-image-analysis-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Image Analysis API
  slug: amazon-rekognition-image-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-image-analysis-api-openapi.yml
- filename: amazon-rekognition-stored-video-analysis-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Stored Video Analysis API
  slug: amazon-rekognition-stored-video-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-stored-video-analysis-api-openapi.yml
- filename: amazon-rekognition-text-detection-api-openapi.yml
  format: yaml
  label: Amazon Rekognition Text Detection API
  slug: amazon-rekognition-text-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/openapi/amazon-rekognition-text-detection-api-openapi.yml
consequence_counts:
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Rekognition Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Amazon Rekognition exposes 15 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Rekognition
provider_slug: amazon-rekognition
slug: amazon-rekognition-agentic-access
source_filename: amazon-rekognition-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-rekognition-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 15\n  by_consequence:\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /#DetectLabels\n  method: post\n  operationId: detectLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DetectFaces\n  method: post\n  operationId: detectFaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#CompareFaces\n  method: post\n  operationId: compareFaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DetectText\n  method: post\n  operationId: detectText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DetectModerationLabels\n  method: post\n  operationId: detectModerationLabels\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#RecognizeCelebrities\n  method: post\n  operationId: recognizeCelebrities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#CreateCollection\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#ListCollections\n  method: post\n\
  \  operationId: listCollections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#IndexFaces\n  method: post\n  operationId: indexFaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#SearchFacesByImage\n  method: post\n  operationId: searchFacesByImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /#StartLabelDetection\n  method: post\n  operationId: startLabelDetection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#GetLabelDetection\n  method: post\n  operationId: getLabelDetection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#CreateFaceLivenessSession\n  method: post\n  operationId: createFaceLivenessSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#GetFaceLivenessSessionResults\n  method: post\n  operationId: getFaceLivenessSessionResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DetectCustomLabels\n  method: post\n  operationId: detectCustomLabels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-rekognition/refs/heads/main/agentic-access/amazon-rekognition-agentic-access.yml
summary_line: 15 operations · 15 acting
tags:
- Celebrity Recognition
- Computer-Vision
- Content Moderation
- Custom Labels
- Deep Learning
- Face Liveness
- Facial Recognition
- Image Analysis
- Machine-Learning
- Object Detection
- Text Detection
- Video Analysis
---
