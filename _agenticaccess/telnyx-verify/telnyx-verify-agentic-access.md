---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 6
api_specs:
- filename: telnyx-verify-openapi.yml
  format: yaml
  label: Telnyx Verify Verifications API
  slug: telnyx-verify-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/openapi/telnyx-verify-openapi.yml
- filename: telnyx-verify-openapi.yml
  format: yaml
  label: Telnyx Verify Profiles API
  slug: telnyx-verify-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/openapi/telnyx-verify-openapi.yml
- filename: telnyx-verify-openapi.yml
  format: yaml
  label: Telnyx Number Lookup API
  slug: telnyx-verify-number-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/openapi/telnyx-verify-openapi.yml
consequence_counts:
  read: 6
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Telnyx Verify Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Telnyx Verify API exposes 17 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Telnyx Verify API
provider_slug: telnyx-verify
slug: telnyx-verify-agentic-access
source_filename: telnyx-verify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/telnyx-verify-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 11\n    connected: 6\n  by_consequence:\n    write: 11\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /verifications/sms\n  method: post\n  operationId: createVerificationSms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verifications/call\n  method: post\n  operationId: createVerificationCall\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verifications/flashcall\n  method: post\n  operationId: createVerificationFlashcall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verifications/whatsapp\n  method: post\n  operationId: createVerificationWhatsapp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /verifications/by_phone_number/{phone_number}\n  method: get\n  operationId: listVerificationsByPhoneNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verifications/by_phone_number/{phone_number}/actions/verify\n  method: post\n  operationId: verifyByPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verifications/{verification_id}\n  method: get\n  operationId: retrieveVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verifications/{verification_id}/actions/verify\n  method: post\n  operationId: verifyById\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify_profiles\n  method: get\n  operationId: listVerifyProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify_profiles\n  method: post\n  operationId: createVerifyProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify_profiles/{verify_profile_id}\n  method: get\n  operationId: retrieveVerifyProfile\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify_profiles/{verify_profile_id}\n  method: patch\n  operationId: updateVerifyProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify_profiles/{verify_profile_id}\n  method: delete\n  operationId: deleteVerifyProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify_profiles/templates\n  method: get\n  operationId: listVerifyProfileTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify_profiles/templates\n  method: post\n  operationId: createVerifyProfileTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify_profiles/templates/{template_id}\n  method: patch\n  operationId: updateVerifyProfileTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /number_lookup/{phone_number}\n  method: get\n  operationId: lookupNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telnyx-verify/refs/heads/main/agentic-access/telnyx-verify-agentic-access.yml
summary_line: 17 operations · 11 acting
tags:
- Number Verification
- Phone Verification
- OTP
- 2FA
- Lookup
- Verify
- Number Lookup
- CNAM
- Identity
- Anti-Fraud
---
