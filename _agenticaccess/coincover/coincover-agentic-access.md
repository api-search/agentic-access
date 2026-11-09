---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 4
api_specs:
- filename: coincover-backup-api-openapi.yml
  format: yaml
  label: Coincover Backup API
  slug: coincover-backup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-backup-api-openapi.yml
- filename: coincover-backups-api-openapi.yml
  format: yaml
  label: Coincover Backups API
  slug: coincover-backups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-backups-api-openapi.yml
- filename: coincover-key-api-openapi.yml
  format: yaml
  label: Coincover Key API
  slug: coincover-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-key-api-openapi.yml
- filename: coincover-keys-api-openapi.yml
  format: yaml
  label: Coincover Keys API
  slug: coincover-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-keys-api-openapi.yml
- filename: coincover-partner-api-openapi.yml
  format: yaml
  label: Coincover Partner API
  slug: coincover-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-partner-api-openapi.yml
- filename: coincover-secure-api-openapi.yml
  format: yaml
  label: Coincover Secure API
  slug: coincover-secure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-secure-api-openapi.yml
- filename: coincover-verification-api-openapi.yml
  format: yaml
  label: Coincover Verification API
  slug: coincover-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coincover/openapi/coincover-verification-api-openapi.yml
consequence_counts:
  read: 4
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coincover Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Coincover exposes 21 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Coincover
provider_slug: coincover
slug: coincover-agentic-access
source_filename: coincover-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/coincover-backup-api-openapi.yml, openapi/coincover-backups-api-openapi.yml,\n  openapi/coincover-key-api-openapi.yml, openapi/coincover-keys-api-openapi.yml, openapi/coincover-partner-api-openapi.yml,\n  openapi/coincover-secure-api-openapi.yml, openapi/coincover-verification-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 17\n    connected: 4\n  by_consequence:\n    write: 17\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/backup/{backupid}\n  method: post\n  operationId: post_v1_backup_backupid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/secure/data\n  method: post\n  operationId: storeSecureData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/secure/file\n  method: post\n  operationId: storeSecureFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/backups/{backupId}/verify\n  method: get\n  operationId: verifyBackup\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/backup/store\n  method: post\n  operationId: storeBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/backup/recover\n  method: post\n  operationId: recoverBackup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/partner/secure/data\n  method: post\n  operationId: partnerStoreSecureData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/partner/secure/file\n  method: post\n  operationId: partnerStoreSecureFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/key/generate\n  method: post\n  operationId: post_v1_key_generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys\n  method: post\n  operationId: assignKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/{keyId}/verify\n  method: get\n  operationId: verifyKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/key/generate\n  method: post\n  operationId: generateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/partner/keys\n  method: post\n  operationId: partnerAssignKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/partner/keys\n  method: get\n  operationId: get_v1_partner_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/partner/keys\n  method: post\n  operationId: post_v1_partner_keys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/partner/secure/{secureid}\n  method: post\n  operationId: post_v1_partner_secure_secureid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/secure/{secureid}\n  method: post\n  operationId: post_v1_secure_secureid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verification/start\n  method: post\n  operationId: startVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verification/status\n  method: get\n  operationId: getVerificationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/verification/simulate\n  method: post\n  operationId: simulateVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verification/{verificationid}\n  method: post\n  operationId: post_v1_verification_verificationid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/coincover/agentic-access/coincover-agentic-access.yml
summary_line: 21 operations · 17 acting
tags:
- Company
- Cryptocurrency
- Security
- Recovery
- Fintech
---
