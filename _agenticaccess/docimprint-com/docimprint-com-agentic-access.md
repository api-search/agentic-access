---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 21
api_specs:
- filename: docimprint-com-billing-api-openapi.yml
  format: yaml
  label: DocImprint Billing API
  slug: docimprint-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-billing-api-openapi.yml
- filename: docimprint-com-check-claims-api-openapi.yml
  format: yaml
  label: DocImprint Check Claims API
  slug: docimprint-com-check-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-check-claims-api-openapi.yml
- filename: docimprint-com-checkpoints-api-openapi.yml
  format: yaml
  label: DocImprint Checkpoints API
  slug: docimprint-com-checkpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-checkpoints-api-openapi.yml
- filename: docimprint-com-collections-api-openapi.yml
  format: yaml
  label: DocImprint Collections API
  slug: docimprint-com-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-collections-api-openapi.yml
- filename: docimprint-com-describe-api-openapi.yml
  format: yaml
  label: DocImprint Describe API
  slug: docimprint-com-describe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-describe-api-openapi.yml
- filename: docimprint-com-extract-api-openapi.yml
  format: yaml
  label: DocImprint Extract API
  slug: docimprint-com-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-extract-api-openapi.yml
- filename: docimprint-com-feedback-api-openapi.yml
  format: yaml
  label: DocImprint Feedback API
  slug: docimprint-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-feedback-api-openapi.yml
- filename: docimprint-com-jobs-api-openapi.yml
  format: yaml
  label: DocImprint Jobs API
  slug: docimprint-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-jobs-api-openapi.yml
- filename: docimprint-com-keys-api-openapi.yml
  format: yaml
  label: DocImprint Keys API
  slug: docimprint-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-keys-api-openapi.yml
- filename: docimprint-com-monitor-api-openapi.yml
  format: yaml
  label: DocImprint Monitor API
  slug: docimprint-com-monitor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-monitor-api-openapi.yml
- filename: docimprint-com-qa-api-openapi.yml
  format: yaml
  label: DocImprint Qa API
  slug: docimprint-com-qa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-qa-api-openapi.yml
- filename: docimprint-com-quickstart-api-openapi.yml
  format: yaml
  label: DocImprint Quickstart API
  slug: docimprint-com-quickstart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-quickstart-api-openapi.yml
- filename: docimprint-com-quota-api-openapi.yml
  format: yaml
  label: DocImprint Quota API
  slug: docimprint-com-quota-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-quota-api-openapi.yml
- filename: docimprint-com-summarize-api-openapi.yml
  format: yaml
  label: DocImprint Summarize API
  slug: docimprint-com-summarize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-summarize-api-openapi.yml
- filename: docimprint-com-translate-api-openapi.yml
  format: yaml
  label: DocImprint Translate API
  slug: docimprint-com-translate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-translate-api-openapi.yml
consequence_counts:
  read: 21
  safety-critical: 1
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Docimprint Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/extract/{id}/revoke
operation_count: 47
overview: 'DocImprint exposes 47 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 25 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DocImprint
provider_slug: docimprint-com
slug: docimprint-com-agentic-access
source_filename: docimprint-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/docimprint-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    acting: 26\n    connected: 21\n  by_consequence:\n    write: 25\n    read: 21\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/extract\n  method: post\n  operationId: extract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}\n  method: get\n  operationId: getBundle\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}\n  method: delete\n  operationId: deleteBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/verify\n  method: get\n  operationId: verifyBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/history\n  method: get\n  operationId: bundleHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/hold\n  method: put\n  operationId: setLegalHold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/hold\n  method: delete\n  operationId: removeLegalHold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/verify-citation\n  method: post\n  operationId: verifyCitation\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/revoke\n  method: post\n  operationId: revokeAttestation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/manifest\n  method: get\n  operationId: getManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/provenance\n\
  \  method: get\n  operationId: getProvenance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/provenance\n  method: post\n  operationId: addProvenance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/handoff\n  method: post\n  operationId: agentHandoff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    -\
  \ read\n    - write\n- path: /v1/extract/{id}/chain\n  method: get\n  operationId: bundleVersionChain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/receipts\n  method: get\n  operationId: listActionReceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/extract/receipts/{receiptId}/verify\n  method: get\n  operationId: verifyActionReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/keys\n  method: get\n  operationId: listSigningKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/download\n  method: get\n  operationId: downloadBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/extract/{id}/notarize\n  method: post\n  operationId: notarizeBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/jobs\n  method: post\n  operationId: createBatchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/collections\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/collections\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n\
  \    - write\n- path: /v1/collections/{id}/search\n  method: get\n  operationId: searchCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/collections/{id}\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/collections/{id}/documents\n  method: post\n  operationId: addCollectionDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/collections/{id}/documents/{bundleId}\n\
  \  method: delete\n  operationId: removeCollectionDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/collections/{id}/documents/{bundleId}/reindex\n  method: post\n  operationId: reindexCollectionDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/collections/{id}/ask\n  method: post\n  operationId: askCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/summarize\n  method: post\n  operationId: summarize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/qa\n  method: post\n  operationId: qa\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/translate\n  method: post\n  operationId: translate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/check-claims\n  method: post\n  operationId: checkClaims\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/describe\n  method: post\n  operationId: describe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/quota\n  method: get\n  operationId: getQuota\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/monitor\n  method: post\n  operationId: createMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/monitor\n  method: get\n  operationId: listMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/monitor/{id}\n  method: get\n  operationId:\
  \ getMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/monitor/{id}\n  method: delete\n  operationId: deleteMonitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/monitor/{id}/history\n  method: get\n  operationId: monitorHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/checkpoints\n  method: post\n  operationId: createCheckpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/checkpoints/{id}\n  method: get\n  operationId: getCheckpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/checkpoints/proof\n  method: get\n  operationId: getCheckpointProof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n    - write\n- path: /v1/checkpoints/public-key\n  method: get\n  operationId: getCheckpointPublicKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - read\n    - write\n- path: /v1/quickstart/sample-bundle\n  method: post\n  operationId: createSampleBundle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/billing/portal\n  method: post\n  operationId: billingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n- path: /v1/feedback\n  method: post\n  operationId: submitFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n    - write\n"
source_yaml_url: https://artifacts.apis.io/docimprint-com/agentic-access/docimprint-com-agentic-access.yml
summary_line: 47 operations · 26 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- Documents
- Verification
- Cryptography
- Payments
- Company
---
