---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 9
api_specs:
- filename: kaiv-ai-account-api-openapi.yml
  format: yaml
  label: kaiv-ai Account API
  slug: kaiv-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-account-api-openapi.yml
- filename: kaiv-ai-activity-api-openapi.yml
  format: yaml
  label: kaiv-ai Activity API
  slug: kaiv-ai-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-activity-api-openapi.yml
- filename: kaiv-ai-changes-api-openapi.yml
  format: yaml
  label: kaiv-ai Changes API
  slug: kaiv-ai-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-changes-api-openapi.yml
- filename: kaiv-ai-credentials-api-openapi.yml
  format: yaml
  label: kaiv-ai Credentials API
  slug: kaiv-ai-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-credentials-api-openapi.yml
- filename: kaiv-ai-documents-api-openapi.yml
  format: yaml
  label: kaiv-ai Documents API
  slug: kaiv-ai-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-documents-api-openapi.yml
- filename: kaiv-ai-keys-api-openapi.yml
  format: yaml
  label: kaiv-ai Keys API
  slug: kaiv-ai-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-keys-api-openapi.yml
- filename: kaiv-ai-no-account-api-openapi.yml
  format: yaml
  label: kaiv-ai No account API
  slug: kaiv-ai-no-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-no-account-api-openapi.yml
- filename: kaiv-ai-policies-api-openapi.yml
  format: yaml
  label: kaiv-ai Policies API
  slug: kaiv-ai-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-policies-api-openapi.yml
- filename: kaiv-ai-servers-api-openapi.yml
  format: yaml
  label: kaiv-ai Servers API
  slug: kaiv-ai-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-servers-api-openapi.yml
consequence_counts:
  read: 9
  safety-critical: 2
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Kaiv Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /session
operation_count: 31
overview: 'kaiv-ai exposes 31 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 20 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: kaiv-ai
provider_slug: kaiv-ai
slug: kaiv-ai-agentic-access
source_filename: kaiv-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/kaiv-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 9\n    acting: 22\n  by_consequence:\n    read: 9\n    safety-critical: 2\n    write: 20\n  human_in_the_loop_required: 2\noperations:\n- path: /whoami\n  method: get\n  operationId: whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /session\n  method: delete\n  operationId: signOut\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /servers\n  method: get\n  operationId: listServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers\n  method: post\n  operationId: createServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}\n  method: get\n  operationId: getServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/{id}\n  method: delete\n  operationId: deleteServer\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}/spec\n  method: put\n  operationId: replaceSpec\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}/introspect\n  method: post\n  operationId: introspectServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}/tls\n  method: patch\n  operationId: setDatabaseTls\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}/api-base\n  method: patch\n  operationId: setApiBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}/tools\n  method: patch\n  operationId: setToolsExposed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}/tools/{toolId}\n\
  \  method: patch\n  operationId: setToolExposed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}/publish\n  method: post\n  operationId: publishServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}/upstream-auth\n  method: put\n  operationId: setServerCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /servers/{id}/upstream-auth/test\n  method: post\n  operationId: testServerCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}/revisions\n  method: get\n  operationId: listRevisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/{id}/revisions/{revId}/promote\n  method: post\n  operationId: promoteRevision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /servers/{id}/revisions/{revId}/reject\n  method: post\n  operationId: rejectRevision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}/auto-promote\n  method: post\n  operationId: setAutoPromote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{id}/tools/{toolId}/invoke\n  method: post\n  operationId: invokeTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/servers\n  method: post\n  operationId: createDocumentsServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/servers/{id}\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/servers/{id}/documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /keys\n  method: post\n  operationId: createGatewayKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys/{id}\n  method: delete\n  operationId: revokeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /policies\n\
  \  method: get\n  operationId: listPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies\n  method: post\n  operationId: createPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audit\n  method: get\n  operationId: listToolCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claimable\n  method: post\n  operationId: createTrialServer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/kaiv-ai/agentic-access/kaiv-ai-agentic-access.yml
summary_line: 31 operations · 22 acting · 2 human-in-the-loop
tags:
- Artificial Intelligence
- Infrastructure
- MCP
- Bridge
- Enterprise
- Developer Tools
---
