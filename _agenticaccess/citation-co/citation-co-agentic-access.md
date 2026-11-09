---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 21
api_specs:
- filename: citation-co-balance-api-openapi.yml
  format: yaml
  label: Citation Balance API
  slug: citation-co-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-balance-api-openapi.yml
- filename: citation-co-checks-api-openapi.yml
  format: yaml
  label: Citation Checks API
  slug: citation-co-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-checks-api-openapi.yml
- filename: citation-co-documents-api-openapi.yml
  format: yaml
  label: Citation Documents API
  slug: citation-co-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-documents-api-openapi.yml
- filename: citation-co-events-api-openapi.yml
  format: yaml
  label: Citation Events API
  slug: citation-co-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-events-api-openapi.yml
- filename: citation-co-exports-api-openapi.yml
  format: yaml
  label: Citation Exports API
  slug: citation-co-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-exports-api-openapi.yml
- filename: citation-co-files-api-openapi.yml
  format: yaml
  label: Citation Files API
  slug: citation-co-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-files-api-openapi.yml
- filename: citation-co-imports-api-openapi.yml
  format: yaml
  label: Citation Imports API
  slug: citation-co-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-imports-api-openapi.yml
- filename: citation-co-jobs-api-openapi.yml
  format: yaml
  label: Citation Jobs API
  slug: citation-co-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-jobs-api-openapi.yml
- filename: citation-co-ledger-api-openapi.yml
  format: yaml
  label: Citation Ledger API
  slug: citation-co-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-ledger-api-openapi.yml
- filename: citation-co-me-api-openapi.yml
  format: yaml
  label: Citation Me API
  slug: citation-co-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-me-api-openapi.yml
- filename: citation-co-pricing-api-openapi.yml
  format: yaml
  label: Citation Pricing API
  slug: citation-co-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-pricing-api-openapi.yml
- filename: citation-co-sources-api-openapi.yml
  format: yaml
  label: Citation Sources API
  slug: citation-co-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-sources-api-openapi.yml
- filename: citation-co-webhooks-api-openapi.yml
  format: yaml
  label: Citation Webhooks API
  slug: citation-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-webhooks-api-openapi.yml
- filename: citation-co-write-api-openapi.yml
  format: yaml
  label: Citation Write API
  slug: citation-co-write-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-write-api-openapi.yml
consequence_counts:
  read: 21
  safety-critical: 1
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Citation Co Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /documents/{document_id}/invitations/{invitation_id}
operation_count: 47
overview: 'Citation exposes 47 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 25 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Citation
provider_slug: citation-co
slug: citation-co-agentic-access
source_filename: citation-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/citation-co-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 21\n    acting: 26\n  by_consequence:\n    read: 21\n    write: 25\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /me\n  method: get\n  operationId: connection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: pricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance\n  method: get\n  operationId:\
  \ balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ledger\n  method: get\n  operationId: ledger\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}\n  method: get\n  operationId: readDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}\n  method: patch\n  operationId: updateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}\n  method: delete\n  operationId: trashDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/restore\n  method: post\n  operationId: restoreDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/history\n  method: get\n  operationId: history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/history/{history_id}\n  method: get\n  operationId: historyEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/sources\n  method: get\n  operationId: listSources\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/sources\n  method: post\n  operationId: addSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/sources/{source_id}\n  method: get\n  operationId: readSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/sources/{source_id}\n  method: patch\n  operationId: updateSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/citations\n  method: post\n  operationId: insertCitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/bibliography\n  method: get\n  operationId: bibliography\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/citation-check\n  method: get\n  operationId: checkCitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/writing-context\n  method: get\n\
  \  operationId: writingContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/writing-context\n  method: patch\n  operationId: saveWritingContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write\n  method: post\n  operationId: writeJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checks\n  method: post\n  operationId: checkJob\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sources/resolve\n  method: post\n  operationId: resolveJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imports\n  method: post\n  operationId: importJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exports\n  method: post\n  operationId: exportJob\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{job_id}\n  method: get\n  operationId: job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}/cancel\n  method: post\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{job_id}/review\n  method: get\n  operationId: checkReview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /jobs/{job_id}/apply\n  method: post\n  operationId: applyWriting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{job_id}/findings/{finding_id}\n  method: patch\n  operationId: decideFinding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{file_id}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: post\n  operationId: upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{file_id}/download\n  method: get\n  operationId: download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/sharing\n  method: get\n  operationId: sharing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/sharing\n  method: patch\n  operationId: setPublicLink\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/invitations\n  method: post\n  operationId: invite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/invitations/{invitation_id}\n  method: delete\n  operationId: revokeInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /documents/{document_id}/members\n  method: patch\n  operationId: setMemberRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/comments\n  method: get\n  operationId: comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/comments\n  method: post\n  operationId: addComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/comments/{comment_id}/resolve\n\
  \  method: post\n  operationId: resolveComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}/deliveries\n  method: get\n  operationId: webhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/citation-co/agentic-access/citation-co-agentic-access.yml
summary_line: 47 operations · 26 acting · 1 human-in-the-loop
tags:
- Citations
- Bibliography
- WritingTool
- Academic
- Productivity
---
