---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 10
api_specs:
- filename: basecite-com-admin-api-openapi.yml
  format: yaml
  label: BaseCite Admin API
  slug: basecite-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-admin-api-openapi.yml
- filename: basecite-com-ai-api-openapi.yml
  format: yaml
  label: BaseCite AI API
  slug: basecite-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-ai-api-openapi.yml
- filename: basecite-com-oauth-api-openapi.yml
  format: yaml
  label: BaseCite OAuth API
  slug: basecite-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-oauth-api-openapi.yml
- filename: basecite-com-organizations-api-openapi.yml
  format: yaml
  label: BaseCite Organizations API
  slug: basecite-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-organizations-api-openapi.yml
- filename: basecite-com-portal-api-openapi.yml
  format: yaml
  label: BaseCite Portal API
  slug: basecite-com-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-portal-api-openapi.yml
- filename: basecite-com-sandbox-api-openapi.yml
  format: yaml
  label: BaseCite Sandbox API
  slug: basecite-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-sandbox-api-openapi.yml
consequence_counts:
  physical: 1
  read: 10
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Basecite Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/organizations/{org_id}/partner-uploads/{upload_id}/withdraw
operation_count: 21
overview: 'BaseCite exposes 21 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 10 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BaseCite
provider_slug: basecite-com
slug: basecite-com-agentic-access
source_filename: basecite-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/basecite-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 10\n    acting: 11\n  by_consequence:\n    read: 10\n    write: 10\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/ai/capabilities\n  method: get\n  operationId: getAiCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox\n  method: get\n  operationId: getSandboxInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /api/v1/sandbox/keys\n  method: get\n  operationId: getSandboxKeyInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sandbox/keys\n  method: post\n  operationId: issueSandboxCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox/echo\n  method: post\n  operationId: sandboxEcho\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sandbox/batch\n  method: post\n  operationId:\
  \ sandboxBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/identity\n  method: get\n  operationId: get__oauth_identity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portal/config\n  method: get\n  operationId: getPortalConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/tenant-keys/policy\n  method: get\n  operationId: getTenantKeyPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/tenant-keys/issue\n  method:\
  \ post\n  operationId: issueTenantKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ai/access-policy\n  method: get\n  operationId: getAiAccessPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/{org_id}/customer-uploads\n  method: post\n  operationId: createCustomerUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_id}/partner-uploads/initiate\n  method:\
  \ post\n  operationId: initiatePartnerUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_id}/partner-uploads/part\n  method: put\n  operationId: uploadPartnerPart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_id}/partner-uploads/complete\n  method: post\n  operationId: completePartnerUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_id}/partner-uploads/{upload_id}\n  method: get\n  operationId: getPartnerUploadStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/{org_id}/partner-uploads/{upload_id}/withdraw\n  method: post\n  operationId: withdrawPartnerUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_id}/customer-uploads/{upload_id}/corrections\n  method: post\n  operationId: createUploadCorrection\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_id}/customer-uploads/{upload_id}/origin-cairn-review\n  method: post\n  operationId: createOriginCairnReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/{org_id}/ai-context/{upload_id}\n  method: get\n  operationId: getAiContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/{org_id}/request-records\n  method: get\n  operationId: listRequestRecords\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/basecite-com/agentic-access/basecite-com-agentic-access.yml
summary_line: 21 operations · 11 acting
tags:
- Company
- Artificial Intelligence
- Evidence
- Platform
- Privacy
---
