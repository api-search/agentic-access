---
acting_count: 20
action_class_counts:
  acting: 20
api_specs:
- filename: amazon-payment-cryptography-openapi.yml
  format: yaml
  label: AWS Payment Cryptography API
  slug: aws-payment-cryptography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/openapi/amazon-payment-cryptography-openapi.yml
consequence_counts:
  safety-critical: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 20
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Payment Cryptography Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.CreateAlias
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.CreateKey
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.DeleteAlias
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.DeleteKey
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.ExportKey
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.GetAlias
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.GetKey
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.GetParametersForExport
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.GetParametersForImport
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.GetPublicKeyCertificate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.ImportKey
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.ListAliases
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.ListKeys
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.ListTagsForResource
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.RestoreKey
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.StartKeyUsage
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.StopKeyUsage
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.TagResource
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.UntagResource
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=PaymentCryptographyControlPlane.UpdateAlias
operation_count: 20
overview: 'Amazon Payment Cryptography exposes 20 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 safety-critical.


  20 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
slug: amazon-payment-cryptography-agentic-access
source_filename: amazon-payment-cryptography-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-payment-cryptography-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 20\n  by_consequence:\n    safety-critical: 20\n  human_in_the_loop_required: 20\noperations:\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.CreateAlias\n  method: post\n  operationId: CreateAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.CreateKey\n\
  \  method: post\n  operationId: CreateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.DeleteAlias\n  method: post\n  operationId: DeleteAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.DeleteKey\n  method: post\n  operationId: DeleteKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.ExportKey\n  method: post\n  operationId: ExportKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.GetAlias\n  method: post\n  operationId: GetAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.GetKey\n  method: post\n  operationId: GetKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.GetParametersForExport\n  method: post\n  operationId: GetParametersForExport\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.GetParametersForImport\n  method: post\n  operationId:\
  \ GetParametersForImport\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.GetPublicKeyCertificate\n  method: post\n  operationId: GetPublicKeyCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.ImportKey\n  method: post\n  operationId: ImportKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.ListAliases\n  method: post\n  operationId: ListAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.ListKeys\n  method: post\n  operationId: ListKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.ListTagsForResource\n  method: post\n  operationId: ListTagsForResource\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.RestoreKey\n  method: post\n  operationId: RestoreKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.StartKeyUsage\n  method:\
  \ post\n  operationId: StartKeyUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.StopKeyUsage\n  method: post\n  operationId: StopKeyUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.TagResource\n  method: post\n  operationId: TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.UntagResource\n  method: post\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=PaymentCryptographyControlPlane.UpdateAlias\n  method: post\n  operationId: UpdateAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-payment-cryptography/refs/heads/main/agentic-access/amazon-payment-cryptography-agentic-access.yml
summary_line: 20 operations · 20 acting · 20 human-in-the-loop
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
---
