---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 2
api_specs:
- filename: certificate-enrolment-protocols-openapi.yml
  format: yaml
  label: ACME - Automatic Certificate Management Environment (RFC 8555)
  slug: acme-rfc-8555
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certificate-enrolment-protocols/refs/heads/main/openapi/certificate-enrolment-protocols-openapi.yml
consequence_counts:
  physical: 3
  read: 2
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Certificate Enrolment Protocols Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /acme/revoke-cert
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /acme/new-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /acme/order/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /acme/order/{id}/finalize
operation_count: 11
overview: 'Certificate Enrolment Protocols exposes 11 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 5 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Certificate Enrolment Protocols
provider_slug: certificate-enrolment-protocols
slug: certificate-enrolment-protocols-agentic-access
source_filename: certificate-enrolment-protocols-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/certificate-enrolment-protocols-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 2\n    acting: 9\n  by_consequence:\n    read: 2\n    write: 5\n    physical: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /directory\n  method: get\n  operationId: getDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /acme/new-nonce\n  method: head\n  operationId: newNonce\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /acme/new-account\n  method: post\n  operationId: newAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acme/new-order\n  method: post\n  operationId: newOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acme/order/{id}\n  method: post\n  operationId: getOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n \
  \     purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acme/order/{id}/finalize\n  method: post\n  operationId: finalizeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acme/authz/{id}\n  method: post\n  operationId: getAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acme/chall/{id}\n  method: post\n  operationId: respondToChallenge\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acme/cert/{id}\n  method: post\n  operationId: downloadCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /acme/revoke-cert\n  method: post\n  operationId: revokeCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /acme/key-change\n  method: post\n  operationId: keyChange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certificate-enrolment-protocols/refs/heads/main/agentic-access/certificate-enrolment-protocols-agentic-access.yml
summary_line: 11 operations · 9 acting · 1 human-in-the-loop
tags:
- ACME
- Automation
- CMP
- Certificates
- Cryptography
- EST
- IETF
- Let's Encrypt
- PKI
- RFC
- Renewal
- SCEP
- Security
- Standards
---
