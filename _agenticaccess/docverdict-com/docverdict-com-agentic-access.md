---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 10
api_specs:
- filename: docverdict-com-analyze-api-openapi.yml
  format: yaml
  label: DocVerdict Analyze API
  slug: docverdict-com-analyze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docverdict-com/openapi/docverdict-com-analyze-api-openapi.yml
- filename: docverdict-com-api-access-api-openapi.yml
  format: yaml
  label: DocVerdict Api Access API
  slug: docverdict-com-api-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docverdict-com/openapi/docverdict-com-api-access-api-openapi.yml
- filename: docverdict-com-artifacts-api-openapi.yml
  format: yaml
  label: DocVerdict Artifacts API
  slug: docverdict-com-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docverdict-com/openapi/docverdict-com-artifacts-api-openapi.yml
- filename: docverdict-com-checkout-api-openapi.yml
  format: yaml
  label: DocVerdict Checkout API
  slug: docverdict-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docverdict-com/openapi/docverdict-com-checkout-api-openapi.yml
- filename: docverdict-com-health-api-openapi.yml
  format: yaml
  label: DocVerdict Health API
  slug: docverdict-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docverdict-com/openapi/docverdict-com-health-api-openapi.yml
- filename: docverdict-com-license-api-openapi.yml
  format: yaml
  label: DocVerdict License API
  slug: docverdict-com-license-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docverdict-com/openapi/docverdict-com-license-api-openapi.yml
- filename: docverdict-com-mcp-api-openapi.yml
  format: yaml
  label: DocVerdict MCP API
  slug: docverdict-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docverdict-com/openapi/docverdict-com-mcp-api-openapi.yml
- filename: docverdict-com-pro-api-openapi.yml
  format: yaml
  label: DocVerdict Pro API
  slug: docverdict-com-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docverdict-com/openapi/docverdict-com-pro-api-openapi.yml
- filename: docverdict-com-report-api-openapi.yml
  format: yaml
  label: DocVerdict Report API
  slug: docverdict-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docverdict-com/openapi/docverdict-com-report-api-openapi.yml
- filename: docverdict-com-stripe-api-openapi.yml
  format: yaml
  label: DocVerdict Stripe API
  slug: docverdict-com-stripe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docverdict-com/openapi/docverdict-com-stripe-api-openapi.yml
- filename: docverdict-com-well-known-api-openapi.yml
  format: yaml
  label: DocVerdict .well Known API
  slug: docverdict-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docverdict-com/openapi/docverdict-com-well-known-api-openapi.yml
consequence_counts:
  physical: 3
  read: 10
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Docverdict Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/api-access
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/pro
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/report
operation_count: 20
overview: 'DocVerdict exposes 20 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 7 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DocVerdict
provider_slug: docverdict-com
slug: docverdict-com-agentic-access
source_filename: docverdict-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/docverdict-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 10\n    acting: 10\n  by_consequence:\n    read: 10\n    write: 7\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyze\n  method: post\n  operationId: analyze_pdf_analyze_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyze/photo\n  method: post\n  operationId: analyze_photo_analyze_photo_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyze/compare\n  method: post\n  operationId: analyze_compare_analyze_compare_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyze/email\n  method: post\n  operationId: analyze_email_analyze_email_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /report/{token}\n  method: get\n  operationId: get_report_report__token__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{token}/pdf\n  method: get\n  operationId: get_report_pdf_report__token__pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{token}/artifact\n  method: get\n  operationId: get_report_artifact_report__token__artifact_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artifacts/{artifact_id}\n  method: get\n\
  \  operationId: get_artifact_artifacts__artifact_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/docverdict-signing-key\n  method: get\n  operationId: signing_key_endpoint__well_known_docverdict_signing_key_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout/report\n  method: post\n  operationId: checkout_report_checkout_report_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/pro\n  method: post\n  operationId: checkout_pro_checkout_pro_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pro/claim\n  method: get\n  operationId: pro_claim_pro_claim_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /license/check\n  method: get\n  operationId: license_check_license_check_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stripe/webhook\n  method: post\n  operationId: stripe_webhook_stripe_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/api-access\n  method: post\n  operationId: checkout_api_access_checkout_api_access_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-access/claim\n  method: get\n  operationId: api_access_claim_api_access_claim_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-access/portal\n  method: post\n  operationId: api_access_portal_api_access_portal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp\n  method: get\n  operationId: mcp_get_api_mcp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: mcp_endpoint_api_mcp_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/docverdict-com/agentic-access/docverdict-com-agentic-access.yml
summary_line: 20 operations · 10 acting
tags:
- Documents
- Forensics
- PDF
- Metadata
- Verification
- Free
---
