---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 16
api_specs:
- filename: gridline-deepfake-api-openapi.yml
  format: yaml
  label: Gridlines Deepfake API
  slug: gridline-deepfake-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-deepfake-api-openapi.yml
- filename: gridline-digilocker-api-openapi.yml
  format: yaml
  label: Gridlines Digilocker API
  slug: gridline-digilocker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-digilocker-api-openapi.yml
- filename: gridline-e-sign-api-openapi.yml
  format: yaml
  label: Gridlines E Sign API
  slug: gridline-e-sign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-e-sign-api-openapi.yml
- filename: gridline-face-api-api-openapi.yml
  format: yaml
  label: Gridlines Face API
  slug: gridline-face-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-face-api-api-openapi.yml
- filename: gridline-individual-api-openapi.yml
  format: yaml
  label: Gridlines Individual API
  slug: gridline-individual-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-individual-api-openapi.yml
- filename: gridline-liveness-api-openapi.yml
  format: yaml
  label: Gridlines Liveness API
  slug: gridline-liveness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-liveness-api-openapi.yml
- filename: gridline-pull-education-documents-api-openapi.yml
  format: yaml
  label: Gridlines Pull Education Documents API
  slug: gridline-pull-education-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-pull-education-documents-api-openapi.yml
- filename: gridline-uidai-ovse-api-openapi.yml
  format: yaml
  label: Gridlines UIDAI OVSE API
  slug: gridline-uidai-ovse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-uidai-ovse-api-openapi.yml
- filename: gridline-utility-api-openapi.yml
  format: yaml
  label: Gridlines Utility API
  slug: gridline-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-utility-api-openapi.yml
- filename: gridline-workflow-mgmt-api-openapi.yml
  format: yaml
  label: Gridlines Workflow Mgmt API
  slug: gridline-workflow-mgmt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridline/openapi/gridline-workflow-mgmt-api-openapi.yml
consequence_counts:
  read: 16
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gridline Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'Gridlines exposes 32 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gridlines
provider_slug: gridline
slug: gridline-agentic-access
source_filename: gridline-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/gridline-aadhaar-openapi.yml, openapi/gridline-digilocker-openapi.yml, openapi/gridline-face-match-openapi.yml,\n  openapi/gridline-journey-orchestrator-openapi.yml, openapi/gridline-liveness-check-openapi.yml,\n  openapi/gridline-profile-lookup-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    acting: 16\n    connected: 16\n  by_consequence:\n    write: 16\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /uidai-api/ovse/generate-qr\n  method: post\n  operationId: post-uidai-api-ovse-generate-qr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uidai-api/ovse/status\n  method: get\n  operationId: get-uidai-api-ovse-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digilocker/init\n  method: post\n  operationId: post-digilocker-init\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digilocker/issued-files\n  method: get\n  operationId: get-digilocker-issued_files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digilocker/issued-file\n\
  \  method: post\n  operationId: post-digilocker-issued_file\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digilocker/eaadhaar\n  method: get\n  operationId: get-digilocker-eaadhaar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digilocker/education/issuers\n  method: get\n  operationId: get-digilocker-education-issuers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /digilocker/education/pull-document\n  method: post\n  operationId: post-digilocker-education-pull-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digilocker/pan/pull-document\n  method: post\n  operationId: post-digilocker-pan-pull-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /digilocker/verify-account\n  method: post\n  operationId: post-digilocker-verify-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /face-api/verify\n  method: post\n  operationId: post-face-api-face-verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflow-mgmt/api/application/init\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflow-mgmt/api/application/{application_id}/details\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflow-mgmt/api/application/{application_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /liveness/passive-check\n\
  \  method: post\n  operationId: post-liveness-passive-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile-api/individual/educational-document-ocr\n  method: post\n  operationId: post-profile-api-individual-educational-document-ocr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile-api/utility/fetch-digipin-from-lat-long\n  method: post\n  operationId: post-profile-api-utility-fetch-digipin-from-lat-long\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /profile-api/address/geocode\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile-api/address/reverse-geocode\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile-api/utility/fetch-lat-long-from-digipin\n  method: post\n  operationId: post-profile-api-utility-fetch-lat-long-from-digipin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /profile-api/utility/fetch-distance-between-digipins\n  method: post\n  operationId: post-profile-api-utility-fetch-distance-between-digipins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile-api/utility/string-compare\n  method: post\n  operationId: post-profile-api-utility-string-compare-api\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile-api/deepfake/image/init\n  method: post\n  operationId: post-profile-api-deepfake-image-init\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile-api/deepfake/image/status\n  method: get\n  operationId: get-profile-api-deepfake-image-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile-api/deepfake/video/init\n  method: post\n  operationId: post-profile-api-deepfake-video-init\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile-api/deepfake/video/status\n  method: get\n  operationId: get-profile-api-deepfake-video-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /profile-api/deepfake/audio/init\n  method: post\n  operationId: post-profile-api-deepfake-audio-init\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile-api/deepfake/audio/status\n  method: get\n  operationId: get-profile-api-deepfake-audio-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile-api/esign/init\n  method: post\n  operationId: post-profile-api-esign-init\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /profile-api/esign/fetch-document-signed\n  method: get\n  operationId: post-profile-api-esign-fetch-document-signed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile-api/esign/status\n  method: get\n  operationId: post-profile-api-esign-fetch-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile-api/esign/audit-trail\n  method: get\n  operationId: post-profile-api-esign-fetch-audit-trail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/gridline/agentic-access/gridline-agentic-access.yml
summary_line: 32 operations · 16 acting
tags:
- Company
- Onboarding
- Identity Verification
- KYC
- eSigning
- Fraud Prevention
- VideoKYC
- DigitalOnboarding
- Fintech
---
