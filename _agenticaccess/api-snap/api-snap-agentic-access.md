---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: api-snap-openapi.yml
  format: yaml
  label: QR Code API
  slug: qr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: Screenshot API
  slug: screenshot
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: Image Resize API
  slug: resize
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: PDF API
  slug: pdf
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: Markdown API
  slug: markdown
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: URL Metadata API
  slug: meta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: Hash API
  slug: hash
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: JWT Decode API
  slug: jwt-decode
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: Base64 API
  slug: base64
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: UUID API
  slug: uuid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: Color API
  slug: color
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: Lorem Ipsum API
  slug: lorem
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
- filename: api-snap-openapi.yml
  format: yaml
  label: Placeholder Image API
  slug: placeholder
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-openapi.yml
consequence_counts:
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Api Snap Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'API Snap exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: API Snap
provider_slug: api-snap
slug: api-snap-agentic-access
source_filename: api-snap-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/api-snap-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 8\n    acting: 6\n  by_consequence:\n    read: 8\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/qr\n  method: get\n  operationId: generateQrCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/resize\n  method: post\n  operationId: resizeImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/screenshot\n  method: get\n  operationId: captureScreenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pdf\n  method: post\n  operationId: htmlToPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hash\n  method: get\n  operationId: hashStringGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hash\n  method: post\n  operationId: hashStringPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/uuid\n  method: get\n  operationId: generateId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/meta\n  method: get\n  operationId: extractUrlMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/base64\n  method: post\n  operationId: base64EncodeDecode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/jwt-decode\n  method: post\n  operationId:\
  \ decodeJwt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/color\n  method: get\n  operationId: convertColor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/lorem\n  method: get\n  operationId: generateLoremIpsum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/markdown\n  method: post\n  operationId: markdownToHtml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/placeholder\n  method: get\n  operationId: generatePlaceholderImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/agentic-access/api-snap-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- API Utilities
- Developer Tools
- QR Codes
- Screenshots
- Image Processing
- PDF Generation
- Markdown
- URL Metadata
- Hashing
- JWT
- Base64
- UUID
- Color Conversion
- Lorem Ipsum
- Placeholder Images
---
