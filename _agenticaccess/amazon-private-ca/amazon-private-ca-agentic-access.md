---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 7
api_specs:
- filename: amazon-private-ca-aws-certificate-manager-private-certificate-authority-api-openapi.yml
  format: yaml
  label: Amazon Private CA AWS Certificate Manager Private Certificate Authority API
  slug: amazon-private-ca-aws-certificate-manager-private-certificate-authority-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/openapi/amazon-private-ca-aws-certificate-manager-private-certificate-authority-api-openapi.yml
consequence_counts:
  read: 7
  safety-critical: 1
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Private Ca Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=ACMPrivateCA.RevokeCertificate
operation_count: 23
overview: 'Amazon Private CA exposes 23 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 15 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
slug: amazon-private-ca-agentic-access
source_filename: amazon-private-ca-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/amazon-private-ca-x-amz-target-acmprivateca-createcertificateauthority-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-createcertificateauthorityauditreport-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-createpermission-api-openapi.yml, openapi/amazon-private-ca-x-amz-target-acmprivateca-deletecertificateauthority-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-deletepermission-api-openapi.yml, openapi/amazon-private-ca-x-amz-target-acmprivateca-deletepolicy-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-describecertificateauthority-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-describecertificateauthorityauditreport-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-getcertificate-api-openapi.yml, openapi/amazon-private-ca-x-amz-target-acmprivateca-getcertificateauthoritycertificate-api-openapi.yml,\n\
  \  openapi/amazon-private-ca-x-amz-target-acmprivateca-getcertificateauthoritycsr-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-getpolicy-api-openapi.yml, openapi/amazon-private-ca-x-amz-target-acmprivateca-importcertificateauthoritycertificate-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-issuecertificate-api-openapi.yml, openapi/amazon-private-ca-x-amz-target-acmprivateca-listcertificateauthorities-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-listpermissions-api-openapi.yml, openapi/amazon-private-ca-x-amz-target-acmprivateca-listtags-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-putpolicy-api-openapi.yml, openapi/amazon-private-ca-x-amz-target-acmprivateca-restorecertificateauthority-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-revokecertificate-api-openapi.yml, openapi/amazon-private-ca-x-amz-target-acmprivateca-tagcertificateauthority-api-openapi.yml,\n\
  \  openapi/amazon-private-ca-x-amz-target-acmprivateca-untagcertificateauthority-api-openapi.yml,\n  openapi/amazon-private-ca-x-amz-target-acmprivateca-updatecertificateauthority-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 16\n    connected: 7\n  by_consequence:\n    write: 15\n    read: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /#X-Amz-Target=ACMPrivateCA.CreateCertificateAuthority\n  method: post\n  operationId: CreateCertificateAuthority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.CreateCertificateAuthorityAuditReport\n  method: post\n  operationId: CreateCertificateAuthorityAuditReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.CreatePermission\n  method: post\n  operationId: CreatePermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.DeleteCertificateAuthority\n  method: post\n  operationId: DeleteCertificateAuthority\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.DeletePermission\n  method: post\n  operationId: DeletePermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.DeletePolicy\n  method: post\n  operationId: DeletePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /#X-Amz-Target=ACMPrivateCA.DescribeCertificateAuthority\n  method: post\n  operationId: DescribeCertificateAuthority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.DescribeCertificateAuthorityAuditReport\n  method: post\n  operationId: DescribeCertificateAuthorityAuditReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.GetCertificate\n  method: post\n  operationId: GetCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=ACMPrivateCA.GetCertificateAuthorityCertificate\n  method: post\n  operationId: GetCertificateAuthorityCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=ACMPrivateCA.GetCertificateAuthorityCsr\n  method: post\n  operationId: GetCertificateAuthorityCsr\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=ACMPrivateCA.GetPolicy\n  method: post\n  operationId: GetPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=ACMPrivateCA.ImportCertificateAuthorityCertificate\n  method: post\n  operationId: ImportCertificateAuthorityCertificate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.IssueCertificate\n  method: post\n  operationId: IssueCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.ListCertificateAuthorities\n  method: post\n  operationId: ListCertificateAuthorities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=ACMPrivateCA.ListPermissions\n  method: post\n  operationId:\
  \ ListPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=ACMPrivateCA.ListTags\n  method: post\n  operationId: ListTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=ACMPrivateCA.PutPolicy\n  method: post\n  operationId: PutPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.RestoreCertificateAuthority\n  method: post\n  operationId: RestoreCertificateAuthority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.RevokeCertificate\n  method: post\n  operationId: RevokeCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.TagCertificateAuthority\n  method: post\n  operationId: TagCertificateAuthority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.UntagCertificateAuthority\n\
  \  method: post\n  operationId: UntagCertificateAuthority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=ACMPrivateCA.UpdateCertificateAuthority\n  method: post\n  operationId: UpdateCertificateAuthority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/agentic-access/amazon-private-ca-agentic-access.yml
summary_line: 23 operations · 16 acting · 1 human-in-the-loop
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
---
