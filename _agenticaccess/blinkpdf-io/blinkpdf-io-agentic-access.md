---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 11
api_specs:
- filename: blinkpdf-io-account-api-openapi.yml
  format: yaml
  label: blinkpdf-io Account API
  slug: blinkpdf-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-account-api-openapi.yml
- filename: blinkpdf-io-compose-api-openapi.yml
  format: yaml
  label: blinkpdf-io Compose API
  slug: blinkpdf-io-compose-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-compose-api-openapi.yml
- filename: blinkpdf-io-discovery-api-openapi.yml
  format: yaml
  label: blinkpdf-io Discovery API
  slug: blinkpdf-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-discovery-api-openapi.yml
- filename: blinkpdf-io-docs-api-openapi.yml
  format: yaml
  label: blinkpdf-io Docs API
  slug: blinkpdf-io-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-docs-api-openapi.yml
- filename: blinkpdf-io-fill-api-openapi.yml
  format: yaml
  label: blinkpdf-io Fill API
  slug: blinkpdf-io-fill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-fill-api-openapi.yml
- filename: blinkpdf-io-fonts-api-openapi.yml
  format: yaml
  label: blinkpdf-io Fonts API
  slug: blinkpdf-io-fonts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-fonts-api-openapi.yml
- filename: blinkpdf-io-health-api-openapi.yml
  format: yaml
  label: blinkpdf-io Health API
  slug: blinkpdf-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-health-api-openapi.yml
- filename: blinkpdf-io-layoutdocument-api-openapi.yml
  format: yaml
  label: blinkpdf-io Layout Document API
  slug: blinkpdf-io-layoutdocument-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-layoutdocument-api-openapi.yml
- filename: blinkpdf-io-pages-api-openapi.yml
  format: yaml
  label: blinkpdf-io Pages API
  slug: blinkpdf-io-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-pages-api-openapi.yml
- filename: blinkpdf-io-read-api-openapi.yml
  format: yaml
  label: blinkpdf-io Read API
  slug: blinkpdf-io-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-read-api-openapi.yml
- filename: blinkpdf-io-render-api-openapi.yml
  format: yaml
  label: blinkpdf-io Render API
  slug: blinkpdf-io-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-render-api-openapi.yml
- filename: blinkpdf-io-sandwichdocument-api-openapi.yml
  format: yaml
  label: blinkpdf-io Sandwich Document API
  slug: blinkpdf-io-sandwichdocument-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-sandwichdocument-api-openapi.yml
- filename: blinkpdf-io-stamp-api-openapi.yml
  format: yaml
  label: blinkpdf-io Stamp API
  slug: blinkpdf-io-stamp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-stamp-api-openapi.yml
- filename: blinkpdf-io-templates-api-openapi.yml
  format: yaml
  label: blinkpdf-io Templates API
  slug: blinkpdf-io-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkpdf-io/openapi/blinkpdf-io-templates-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blinkpdf Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/pages
operation_count: 32
overview: 'blinkpdf-io exposes 32 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 20 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: blinkpdf-io
provider_slug: blinkpdf-io
slug: blinkpdf-io-agentic-access
source_filename: blinkpdf-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/blinkpdf-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 11\n    acting: 21\n  by_consequence:\n    read: 11\n    write: 20\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /openapi.json\n  method: get\n  operationId: publicOpenApiDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs\n  method: get\n  operationId: getDocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method:\
  \ get\n  operationId: livenessProbe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/ready\n  method: get\n  operationId: readinessProbe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: discoveryRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/render\n  method: post\n  operationId: renderMarkdown\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/render/validate\n  method: post\n  operationId:\
  \ validateRenderBody\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/compose\n  method: post\n  operationId: composeDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/compose/validate\n  method: post\n  operationId: validateComposeBody\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/validate-rewrite\n  method: post\n  operationId: validateRewrite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rewrite\n  method: post\n  operationId: rewriteAcroForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pages/validate\n  method: post\n  operationId: validatePagesPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /v1/pages\n  method: post\n  operationId: pagesPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/stamp\n  method: post\n  operationId: stampPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/read\n  method: post\n  operationId: readPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/plan-repair\n  method: post\n  operationId: planAcroFormRepair\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inspect\n  method: post\n  operationId: inspectForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/validate-fill\n  method: post\n  operationId: validateFill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fill\n  method: post\n  operationId: fillForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates\n  method: post\n  operationId: storeTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates\n  method: patch\n  operationId: updateTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates\n  method: delete\n  operationId: deleteTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/{id}/download\n  method: get\n  operationId: downloadTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fonts\n\
  \  method: get\n  operationId: listFonts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/style-targets\n  method: get\n  operationId: describeStyleTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/themes\n  method: get\n  operationId: listThemes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates/layout-document/render\n  method: post\n  operationId: render_layout_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/layout-document/validate\n  method: post\n  operationId: validate_layout_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/sandwich-document/render\n  method: post\n  operationId: render_sandwich_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/templates/sandwich-document/validate\n\
  \  method: post\n  operationId: validate_sandwich_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/blinkpdf-io/agentic-access/blinkpdf-io-agentic-access.yml
summary_line: 32 operations · 21 acting
tags:
- PDF
- Document Processing
- Software-as-a-Service
- Automation
---
