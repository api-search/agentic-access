---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 17
api_specs:
- filename: v12-documents-api-openapi.yml
  format: yaml
  label: V12 Documents API
  slug: v12-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-documents-api-openapi.yml
- filename: v12-findings-api-openapi.yml
  format: yaml
  label: V12 Findings API
  slug: v12-findings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-findings-api-openapi.yml
- filename: v12-me-api-openapi.yml
  format: yaml
  label: V12 Me API
  slug: v12-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-me-api-openapi.yml
- filename: v12-members-api-openapi.yml
  format: yaml
  label: V12 Members API
  slug: v12-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-members-api-openapi.yml
- filename: v12-repositories-api-openapi.yml
  format: yaml
  label: V12 Repositories API
  slug: v12-repositories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-repositories-api-openapi.yml
- filename: v12-runs-api-openapi.yml
  format: yaml
  label: V12 Runs API
  slug: v12-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-runs-api-openapi.yml
- filename: v12-steers-api-openapi.yml
  format: yaml
  label: V12 Steers API
  slug: v12-steers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-steers-api-openapi.yml
consequence_counts:
  read: 17
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: V12 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /orgs/{org}/runs/{run}/links/{link}
operation_count: 35
overview: 'V12 exposes 35 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 17 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: V12
provider_slug: v12
slug: v12-agentic-access
source_filename: v12-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: generated\nsource: openapi/v12-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 17\n    acting: 18\n  by_consequence:\n    read: 17\n    write: 17\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/members\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /orgs/{org}/steers\n  method: get\n  operationId: listSteers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - repos:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/steers\n  method: post\n  operationId: createSteer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - steers:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/steers/{steer}\n  method: get\n  operationId: getSteer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - repos:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/steers/{steer}\n  method: patch\n  operationId: updateSteer\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - steers:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/steers/{steer}\n  method: delete\n  operationId: archiveSteer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - steers:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/steers/{steer}/restore\n  method: post\n  operationId: restoreSteer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - steers:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/repositories\n  method: get\n  operationId: listRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - repos:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/repositories\n  method: post\n  operationId: addRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - repos:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/repositories/{owner}/{repo}\n  method: get\n  operationId: getRepository\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - repos:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/repositories/{owner}/{repo}/refs\n\
  \  method: get\n  operationId: listRefs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - repos:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/repositories/hosted\n  method: post\n  operationId: createHostedRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - repos:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/repositories/{owner}/{repo}/push-credentials\n  method: post\n  operationId: createPushCredential\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - repos:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/repositories/{owner}/{repo}/findings\n  method: get\n  operationId:\
  \ listRepositoryFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - findings:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/findings\n  method: get\n  operationId: listFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - findings:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/findings\n  method: patch\n  operationId: updateFindings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - findings:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/findings/{finding}\n  method: get\n  operationId: getFinding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - findings:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/findings/{finding}\n  method: patch\n  operationId: updateFinding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - findings:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/findings/{finding}/comments\n  method: post\n  operationId: commentOnFinding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - findings:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/runs\n  method: get\n  operationId: listRuns\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - runs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/runs\n  method: post\n  operationId: startRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - runs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/runs/{run}\n  method: get\n  operationId: getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - runs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/runs/{run}/findings\n  method: get\n  operationId: listRunFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - findings:read\n    - runs:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/runs/estimate\n  method: post\n  operationId: estimateRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - runs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/runs/{run}/cancel\n  method: post\n  operationId: cancelRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - runs:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/runs/{run}/links\n  method: get\n  operationId: listRunLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - runs:share\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/runs/{run}/links\n  method: post\n  operationId: createRunLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - findings:read\n    - runs:share\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/runs/{run}/links/{link}\n  method: patch\n  operationId: updateRunLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - findings:read\n    - runs:share\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/runs/{run}/links/{link}\n  method: delete\n  operationId: revokeRunLink\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - runs:share\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /orgs/{org}/documents/uploads\n  method: post\n  operationId: requestDocumentUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - runs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - runs:write\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - runs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/documents/{document}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - runs:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/documents/{document}\n  method: delete\n  operationId: archiveDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - runs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/v12/agentic-access/v12-agentic-access.yml
summary_line: 35 operations · 18 acting · 1 human-in-the-loop
tags:
- Company
- Security
- DevOps
- Automation
- Code Analysis
---
