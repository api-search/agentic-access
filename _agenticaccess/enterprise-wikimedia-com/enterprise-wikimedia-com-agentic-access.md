---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 72
api_specs:
- filename: enterprise-wikimedia-com-articles-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Articles API
  slug: enterprise-wikimedia-com-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-articles-api-openapi.yml
- filename: enterprise-wikimedia-com-authentication-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Authentication API
  slug: enterprise-wikimedia-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-authentication-api-openapi.yml
- filename: enterprise-wikimedia-com-batches-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Batches API
  slug: enterprise-wikimedia-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-batches-api-openapi.yml
- filename: enterprise-wikimedia-com-codes-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Codes API
  slug: enterprise-wikimedia-com-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-codes-api-openapi.yml
- filename: enterprise-wikimedia-com-languages-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Languages API
  slug: enterprise-wikimedia-com-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-languages-api-openapi.yml
- filename: enterprise-wikimedia-com-namespaces-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Namespaces API
  slug: enterprise-wikimedia-com-namespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-namespaces-api-openapi.yml
- filename: enterprise-wikimedia-com-projects-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Projects API
  slug: enterprise-wikimedia-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-projects-api-openapi.yml
- filename: enterprise-wikimedia-com-realtime-articles-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Realtime Articles API
  slug: enterprise-wikimedia-com-realtime-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-realtime-articles-api-openapi.yml
- filename: enterprise-wikimedia-com-realtime-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Realtime Wikidata API
  slug: enterprise-wikimedia-com-realtime-wikidata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-realtime-wikidata-api-openapi.yml
- filename: enterprise-wikimedia-com-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Snapshots API
  slug: enterprise-wikimedia-com-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-snapshots-api-openapi.yml
- filename: enterprise-wikimedia-com-structured-contents-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Structured Contents API
  slug: enterprise-wikimedia-com-structured-contents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-structured-contents-api-openapi.yml
- filename: enterprise-wikimedia-com-structured-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Structured Snapshots API
  slug: enterprise-wikimedia-com-structured-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-structured-snapshots-api-openapi.yml
- filename: enterprise-wikimedia-com-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata API
  slug: enterprise-wikimedia-com-wikidata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-wikidata-api-openapi.yml
- filename: enterprise-wikimedia-com-wikidata-batches-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata Batches API
  slug: enterprise-wikimedia-com-wikidata-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-wikidata-batches-api-openapi.yml
- filename: enterprise-wikimedia-com-wikidata-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata Snapshots API
  slug: enterprise-wikimedia-com-wikidata-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-wikidata-snapshots-api-openapi.yml
consequence_counts:
  read: 72
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Enterprise Wikimedia Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/token-revoke
operation_count: 79
overview: 'Wikimedia Enterprise exposes 79 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 72 read, 6 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wikimedia Enterprise
provider_slug: enterprise-wikimedia-com
slug: enterprise-wikimedia-com-agentic-access
source_filename: enterprise-wikimedia-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/enterprise-wikimedia-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 79\n  by_action_class:\n    acting: 7\n    connected: 72\n  by_consequence:\n    write: 6\n    safety-critical: 1\n    read: 72\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/login\n  method: post\n  operationId: v1-login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/token-refresh\n  method: post\n  operationId: v1-token-refresh\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/token-revoke\n  method: post\n  operationId: v1-token-revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/forgot-password\n  method: post\n  operationId: v1-forgot-password\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/forgot-password-confirm\n  method: post\n  operationId: v1-forgot-password-confirm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/change-password\n  method: post\n  operationId: v1-change-password\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/new-password-required\n  method: post\n  operationId: v1-new-password-required\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/codes\n  method: get\n  operationId: getCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/codes\n  method: post\n  operationId: queryCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/codes/{identifier}\n  method: get\n  operationId: getCodesByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/codes/{identifier}\n  method: post\n  operationId: queryCodesByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/languages\n  method:\
  \ get\n  operationId: getLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/languages\n  method: post\n  operationId: queryLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/languages/{identifier}\n  method: get\n  operationId: getLanguagesByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/languages/{identifier}\n  method: post\n  operationId: queryLanguagesByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects\n  method: get\n  operationId: getProjects\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects\n  method: post\n  operationId: queryProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{identifier}\n  method: get\n  operationId: getProjectsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{identifier}\n  method: post\n  operationId: queryProjectsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/namespaces\n  method: get\n  operationId: getNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/namespaces\n\
  \  method: post\n  operationId: queryNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/namespaces/{identifier}\n  method: get\n  operationId: getNamespacesByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/namespaces/{identifier}\n  method: post\n  operationId: queryNamespacesByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/batches/{date}/{hour}\n  method: get\n  operationId: getBatchesByDateByHour\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/batches/{date}/{hour}\n  method: post\n  operationId: queryBatchesByDateByHour\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/batches/{date}/{hour}/{identifier}\n  method: get\n  operationId: getBatchesByDateByHourByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/batches/{date}/{hour}/{identifier}\n  method: post\n  operationId: queryBatchesByDateByHourByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/batches/{date}/{hour}/{identifier}/download\n  method: head\n  operationId: headBatchesByDateByHourByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/batches/{date}/{hour}/{identifier}/download\n\
  \  method: get\n  operationId: getBatchesByDateByHourByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/batches/{date}/{hour}/wikidata\n  method: get\n  operationId: getBatchesByDateByHourWikidata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/batches/{date}/{hour}/wikidata\n  method: post\n  operationId: queryBatchesByDateByHourWikidata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/batches/{date}/{hour}/wikidata/{identifier}\n  method: get\n  operationId: getBatchesByDateByHourWikidataByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/batches/{date}/{hour}/wikidata/{identifier}\n  method: post\n  operationId: queryBatchesByDateByHourWikidataByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/batches/{date}/{hour}/wikidata/{identifier}/download\n  method: head\n  operationId: headBatchesByDateByHourWikidataByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/batches/{date}/{hour}/wikidata/{identifier}/download\n  method: get\n  operationId: getBatchesByDateByHourWikidataByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots\n  method: get\n  operationId: getSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots\n  method: post\n  operationId: querySnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/{identifier}\n  method: get\n  operationId: getSnapshotsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/{identifier}\n  method: post\n  operationId: querySnapshotsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/{identifier}/download\n  method: head\n  operationId: headSnapshotsByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/{identifier}/download\n  method: get\n  operationId: getSnapshotsByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/{identifier}/chunks\n  method: get\n  operationId: getSnapshotsBySnapshotIdentifierChunks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/{identifier}/chunks\n  method: post\n  operationId: querySnapshotsBySnapshotIdentifierChunks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/{snapshot_identifier}/chunks/{chunk_identifier}\n  method: get\n  operationId: getSnapshotsBySnapshotIdentifierChunksByIdentifier\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/{snapshot_identifier}/chunks/{chunk_identifier}\n  method: post\n  operationId: querySnapshotsBySnapshotIdentifierChunksByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/{snapshot_identifier}/chunks/{chunk_identifier}/download\n  method: head\n  operationId: headSnapshotsBySnapshotIdentifierChunksByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/{snapshot_identifier}/chunks/{chunk_identifier}/download\n  method: get\n  operationId: getSnapshotsBySnapshotIdentifierChunksByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/wikidata\n  method: get\n  operationId: getSnapshotsWikidata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/wikidata\n  method: post\n  operationId: querySnapshotsWikidata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/wikidata/{identifier}\n  method: get\n  operationId: getSnapshotsWikidataByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/wikidata/{identifier}\n  method: post\n  operationId: querySnapshotsWikidataByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /v2/snapshots/wikidata/{identifier}/download\n  method: head\n  operationId: headSnapshotsWikidataByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/wikidata/{identifier}/download\n  method: get\n  operationId: getSnapshotsWikidataByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/wikidata/{identifier}/chunks\n  method: get\n  operationId: getSnapshotsWikidataByIdentifierChunks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/wikidata/{identifier}/chunks\n  method: post\n  operationId: querySnapshotsWikidataByIdentifierChunks\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/wikidata/{identifier}/chunks/{chunk_identifier}\n  method: get\n  operationId: getSnapshotsWikidataByIdentifierChunksByChunkIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/wikidata/{identifier}/chunks/{chunk_identifier}\n  method: post\n  operationId: querySnapshotsWikidataByIdentifierChunksByChunkIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/wikidata/{identifier}/chunks/{chunk_identifier}/download\n  method: head\n  operationId: headSnapshotsWikidataByIdentifierChunksByChunkIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/snapshots/wikidata/{identifier}/chunks/{chunk_identifier}/download\n  method: get\n  operationId: getSnapshotsWikidataByIdentifierChunksByChunkIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/structured-contents\n  method: get\n  operationId: getSnapshotsStructuredContents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/structured-contents\n  method: post\n  operationId: querySnapshotsStructuredContents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/structured-contents/{identifier}\n  method: get\n  operationId: getSnapshotsStructuredContentsByIdentifier\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/structured-contents/{identifier}\n  method: post\n  operationId: querySnapshotsStructuredContentsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/structured-contents/{identifier}/download\n  method: head\n  operationId: headSnapshotsStructuredContentsByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/snapshots/structured-contents/{identifier}/download\n  method: get\n  operationId: getSnapshotsStructuredContentsByIdentifierDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v2/articles/{name}\n  method: get\n  operationId: getArticlesByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/articles/{name}\n  method: post\n  operationId: queryArticlesByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/structured-contents/{name}\n  method: get\n  operationId: getStructuredContentsByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/structured-contents/{name}\n  method: post\n  operationId: queryStructuredContentsByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wikidata/items/{identifier}\n  method: get\n  operationId:\
  \ getWikidataItemsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wikidata/items/{identifier}\n  method: post\n  operationId: queryWikidataItemsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wikidata/properties/{identifier}\n  method: get\n  operationId: getWikidataPropertiesByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wikidata/properties/{identifier}\n  method: post\n  operationId: queryWikidataPropertiesByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wikidata/labels/{identifier}\n  method: get\n\
  \  operationId: getWikidataLabelsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wikidata/labels/{identifier}\n  method: post\n  operationId: queryWikidataLabelsByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/articles\n  method: get\n  operationId: getArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/articles\n  method: post\n  operationId: queryArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wikidata\n  method: get\n  operationId: getWikidata\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wikidata\n  method: post\n  operationId: queryWikidata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/enterprise-wikimedia-com/agentic-access/enterprise-wikimedia-com-agentic-access.yml
summary_line: 79 operations · 7 acting · 1 human-in-the-loop
tags:
- Company
- Data
- Enterprise
- Wikimedia
---
