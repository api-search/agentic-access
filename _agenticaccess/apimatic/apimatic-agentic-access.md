---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 14
api_specs:
- filename: apimatic-docs-portal-api-openapi.yml
  format: yaml
  label: APIMatic Portals API
  slug: apimatic-portals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-docs-portal-api-openapi.yml
- filename: apimatic-sdk-api-openapi.yml
  format: yaml
  label: APIMatic SDK Generation API
  slug: apimatic-sdk-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-sdk-api-openapi.yml
- filename: apimatic-transformation-api-openapi.yml
  format: yaml
  label: APIMatic Transformation API
  slug: apimatic-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-transformation-api-openapi.yml
- filename: apimatic-validation-api-openapi.yml
  format: yaml
  label: APIMatic Validation API
  slug: apimatic-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-validation-api-openapi.yml
consequence_counts:
  read: 14
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apimatic Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'APIMatic exposes 25 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: APIMatic
provider_slug: apimatic
slug: apimatic-agentic-access
source_filename: apimatic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/apimatic-docs-portal-api-openapi.yml, openapi/apimatic-docs-portal-async-api-openapi.yml,\n  openapi/apimatic-sdk-api-openapi.yml, openapi/apimatic-sdk-async-api-openapi.yml, openapi/apimatic-transformation-api-openapi.yml,\n  openapi/apimatic-validation-api-openapi.yml, openapi/apimatic-validation-v2-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    acting: 11\n    connected: 14\n  by_consequence:\n    write: 11\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /portal\n  method: post\n  operationId: generateOnPremPortalViaBuildInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portal/v2\n  method: post\n  operationId: generateOnPremPortalViaBuildInputAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portal/v2/{id}/status\n  method: get\n  operationId: getPortalGenerationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portal/v2/{id}/download\n  method: get\n  operationId: downloadGeneratedPortal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /code-generations/generate-via-file\n  method: post\n  operationId: generateSdkViaFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /code-generations/generate-via-url\n  method: post\n  operationId: generateSdkViaUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /code-generations/{codegen_id}/generated-sdk\n  method: get\n  operationId: downloadSdk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /code-generations\n  method: get\n  operationId: listAllCodeGenerations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /code-generations/{codegen_id}/input-file\n  method: get\n  operationId: downloadInputFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /code-generations/{codegen_id}\n  method: get\n  operationId: getACodeGeneration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /code-generations/{codegen_id}\n  method: delete\n  operationId: deleteCodeGenerationForExternalApis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sdk\n  method: post\n  operationId: generateSdkViaBuildInputAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sdk/{id}/status\n  method: get\n  operationId: getSdkGenerationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sdk/{id}/download\n  method: get\n  operationId: downloadGeneratedSdk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transformations/transform-via-file\n  method: post\n  operationId: transformViaFile\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transformations/transform-via-url\n  method: post\n  operationId: transformViaUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transformations/{transformation_id}/converted-file\n  method: get\n  operationId: downloadTransformedFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transformations/{transformation_id}/input-file\n  method: get\n  operationId: downloadInputFile\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transformations\n  method: get\n  operationId: listAllTransformations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transformations/{transformation_id}\n  method: get\n  operationId: getATransformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transformations/{transformation_id}\n  method: delete\n  operationId: deleteTransformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validation/validate-via-file\n\
  \  method: post\n  operationId: validateApiViaFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validation/validate-via-url\n  method: get\n  operationId: validateApiViaUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /validation/v2/validate-via-file\n  method: post\n  operationId: validateApiViaFileV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validation/v2/validate-via-url\n  method: get\n  operationId:\
  \ validateApiViaUrlV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/agentic-access/apimatic-agentic-access.yml
summary_line: 25 operations · 11 acting
tags:
- API Transformation
- Code Generation
- Developer Experience
- Developer Tools
- Documentation
- SDK Generation
- OpenAPI
---
