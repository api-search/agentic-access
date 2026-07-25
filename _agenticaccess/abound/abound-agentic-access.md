---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 22
api_specs:
- filename: abound-1099-int-api-openapi.yml
  format: yaml
  label: Abound 1099-INT API
  slug: abound-1099-int-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-1099-int-api-openapi.yml
- filename: abound-1099-k-api-openapi.yml
  format: yaml
  label: Abound 1099-K API
  slug: abound-1099-k-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-1099-k-api-openapi.yml
- filename: abound-1099-misc-api-openapi.yml
  format: yaml
  label: Abound 1099-MISC API
  slug: abound-1099-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-1099-misc-api-openapi.yml
- filename: abound-1099-nec-api-openapi.yml
  format: yaml
  label: Abound 1099-NEC API
  slug: abound-1099-nec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-1099-nec-api-openapi.yml
- filename: abound-access-tokens-api-openapi.yml
  format: yaml
  label: Abound Access Tokens API
  slug: abound-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-access-tokens-api-openapi.yml
- filename: abound-electronic-delivery-consents-api-openapi.yml
  format: yaml
  label: Abound Electronic Delivery Consents API
  slug: abound-electronic-delivery-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-electronic-delivery-consents-api-openapi.yml
- filename: abound-mailings-api-openapi.yml
  format: yaml
  label: Abound Mailings API
  slug: abound-mailings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-mailings-api-openapi.yml
- filename: abound-tax-treaties-api-openapi.yml
  format: yaml
  label: Abound Tax Treaties API
  slug: abound-tax-treaties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-tax-treaties-api-openapi.yml
- filename: abound-tin-verifications-api-openapi.yml
  format: yaml
  label: Abound TIN Verifications API
  slug: abound-tin-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-tin-verifications-api-openapi.yml
- filename: abound-users-api-openapi.yml
  format: yaml
  label: Abound Users API
  slug: abound-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-users-api-openapi.yml
- filename: abound-w-8ben-api-openapi.yml
  format: yaml
  label: Abound W-8BEN API
  slug: abound-w-8ben-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-w-8ben-api-openapi.yml
- filename: abound-w-8ben-e-api-openapi.yml
  format: yaml
  label: Abound W-8BEN-E API
  slug: abound-w-8ben-e-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-w-8ben-e-api-openapi.yml
- filename: abound-w-9-api-openapi.yml
  format: yaml
  label: Abound W-9 API
  slug: abound-w-9-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-w-9-api-openapi.yml
consequence_counts:
  read: 22
  write: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Abound Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 55
overview: 'Abound exposes 55 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 33 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Abound
provider_slug: abound
slug: abound-agentic-access
source_filename: abound-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/abound-v4-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    acting: 33\n    connected: 22\n  by_consequence:\n    write: 33\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /v4/access-tokens\n  method: post\n  operationId: accessTokensCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-int\n  method: get\n  operationId: form1099IntList\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/1099-int\n  method: post\n  operationId: form1099IntCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-int/{documentId}\n  method: get\n  operationId: form1099IntRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/1099-int/{documentId}\n  method: delete\n  operationId: form1099IntDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-int/{documentId}/correct\n  method: post\n  operationId: form1099IntCorrect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-int/{documentId}/file\n  method: post\n  operationId: form1099IntFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-int/{documentId}/mail\n  method: post\n  operationId: form1099IntMail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-int/{documentId}/void\n  method: post\n  operationId: form1099IntVoid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-k\n  method: get\n  operationId: form1099KList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/1099-k\n  method: post\n  operationId: form1099KCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-k/{documentId}\n  method: get\n  operationId: form1099KRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/1099-k/{documentId}\n  method: delete\n  operationId: form1099KDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-k/{documentId}/correct\n  method: post\n  operationId: form1099KCorrect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-k/{documentId}/file\n  method: post\n  operationId: form1099KFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-k/{documentId}/mail\n  method: post\n  operationId: form1099KMail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-k/{documentId}/void\n  method: post\n  operationId: form1099KVoid\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-misc\n  method: get\n  operationId: form1099MiscList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/1099-misc\n  method: post\n  operationId: form1099MiscCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-misc/{documentId}\n  method: get\n  operationId: form1099MiscRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/1099-misc/{documentId}\n  method: delete\n  operationId: form1099MiscDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-misc/{documentId}/correct\n  method: post\n  operationId: form1099MiscCorrect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-misc/{documentId}/file\n  method: post\n  operationId: form1099MiscFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-misc/{documentId}/mail\n  method: post\n  operationId: form1099MiscMail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-misc/{documentId}/void\n  method: post\n  operationId: form1099MiscVoid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-nec\n  method:\
  \ get\n  operationId: form1099NecList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/1099-nec\n  method: post\n  operationId: form1099NecCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-nec/{documentId}\n  method: get\n  operationId: form1099NecRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/1099-nec/{documentId}\n  method: delete\n  operationId: form1099NecDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-nec/{documentId}/correct\n  method: post\n  operationId: form1099NecCorrect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-nec/{documentId}/file\n  method: post\n  operationId: form1099NecFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-nec/{documentId}/mail\n  method: post\n  operationId: form1099NecMail\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/1099-nec/{documentId}/void\n  method: post\n  operationId: form1099NecVoid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/w-8ben\n  method: get\n  operationId: formW8benList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/w-8ben\n  method: post\n  operationId: formW8benCreate\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/w-8ben-e\n  method: get\n  operationId: formW8benEList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/w-8ben-e\n  method: post\n  operationId: formW8benECreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/w-8ben-e/{documentId}\n  method: get\n  operationId: formW8benERetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/w-8ben/{documentId}\n  method: get\n  operationId: formW8benRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/w-9\n  method: get\n  operationId: formW9List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/documents/w-9\n  method: post\n  operationId: formW9Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/documents/w-9/{documentId}\n  method: get\n  operationId: formW9Retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/electronic-delivery-consents\n  method: get\n  operationId: electronicDeliveryConsentsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/mailings\n  method: get\n  operationId: mailingsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/mailings/{mailingId}\n  method: get\n  operationId: mailingsRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/mailings/{mailingId}\n  method: put\n  operationId: mailingsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/mailings/{mailingId}\n  method: delete\n  operationId: mailingsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/tax-treaties\n  method: get\n  operationId: taxTreatiesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/tin-verifications\n  method: get\n  operationId: tinVerificationsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/tin-verifications\n  method: post\n  operationId:\
  \ tinVerificationsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/tin-verifications/{tinVerificationId}\n  method: get\n  operationId: tinVerificationsRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/users\n  method: get\n  operationId: usersList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/users\n  method: post\n  operationId: usersCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/users/{userId}\n  method: get\n  operationId: usersRetrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/users/{userId}\n  method: put\n  operationId: usersUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/agentic-access/abound-agentic-access.yml
summary_line: 55 operations · 33 acting
tags:
- Company
- Taxes
- Tax Compliance
- Regulatory Compliance
- Financial Services
- Identity Verification
- Government
- Documents
- Webhooks
- Retired
---
