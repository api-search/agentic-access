---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 11
api_specs:
- filename: finisma-de-konto-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Konto API
  slug: finisma-de-konto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-konto-api-openapi.yml
- filename: finisma-de-kontoausz-ge-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Kontoauszüge API
  slug: finisma-de-kontoausz-ge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-kontoausz-ge-api-openapi.yml
- filename: finisma-de-partner-checks-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Partner Checks API
  slug: finisma-de-partner-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-partner-checks-api-openapi.yml
- filename: finisma-de-rechnungen-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Rechnungen API
  slug: finisma-de-rechnungen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-rechnungen-api-openapi.yml
- filename: finisma-de-selbstauskunft-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Selbstauskunft API
  slug: finisma-de-selbstauskunft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-selbstauskunft-api-openapi.yml
- filename: finisma-de-zahlungsverkehr-api-openapi.yml
  format: yaml
  label: Paulibytes UG (haftungsbeschränkt) Zahlungsverkehr API
  slug: finisma-de-zahlungsverkehr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finisma-de/openapi/finisma-de-zahlungsverkehr-api-openapi.yml
consequence_counts:
  physical: 7
  read: 11
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Finisma De Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /extractions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/axz
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/sepa
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/structure-addresses
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /verify
operation_count: 20
overview: 'Paulibytes UG (haftungsbeschränkt) exposes 20 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 2 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paulibytes UG (haftungsbeschränkt)
provider_slug: finisma-de
slug: finisma-de-agentic-access
source_filename: finisma-de-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: generated\nsource: openapi/finisma-de-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 11\n    acting: 9\n  by_consequence:\n    read: 11\n    physical: 7\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /formats\n  method: get\n  operationId: listFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /codelists/document-types\n  method: get\n  operationId: listDocumentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /codelists/note-subjects\n  method: get\n  operationId: listNoteSubjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /codelists/units\n  method: get\n  operationId: listUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /codelists/vat-categories\n  method: get\n  operationId: listVatCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /codelists/payment-means\n  method: get\n  operationId: listPaymentMeans\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /codelists/attachment-types\n  method: get\n  operationId: listAttachmentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /vat/check\n  method: get\n  operationId: checkVatId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /peppol/check\n  method: get\n  operationId: checkPeppolParticipant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - invoice:create\n\
  \    - invoice:verify\n- path: /verify\n  method: post\n  operationId: verifyInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /me\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /invoices\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /extractions\n  method: post\n  operationId: extractInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /payments/bank-lookup\n  method: get\n  operationId: bankLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /payments/structure-addresses\n  method: post\n  operationId: structureAddresses\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /payments/sepa\n  method: post\n  operationId: createSepaPaymentFile\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /payments/axz\n  method: post\n  operationId: createAxzPaymentFile\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /payments/validate\n  method: post\n  operationId: validatePaymentFile\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /statements/validate\n  method: post\n  operationId: validateBankStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - invoice:create\n    - invoice:verify\n- path: /statements/parse\n  method: post\n  operationId: parseBankStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - invoice:create\n    - invoice:verify\n"
source_yaml_url: https://artifacts.apis.io/finisma-de/agentic-access/finisma-de-agentic-access.yml
summary_line: 20 operations · 9 acting
tags:
- Company
- FinTech
- Invoice
- PDF
- ZUGFeRD
- API
---
