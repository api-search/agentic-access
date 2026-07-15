---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 44
api_specs:
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Associations API
  slug: vantaca-associations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Homeowner Accounts API
  slug: vantaca-homeowner-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Accounts Payable & Ledger API
  slug: vantaca-accounts-payable-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Work Orders API
  slug: vantaca-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Violations & Compliance API
  slug: vantaca-violations-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Architectural Requests (ARC) API
  slug: vantaca-architectural-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
- filename: vantaca-openapi.json
  format: json
  label: Vantaca Vendors & Service Providers API
  slug: vantaca-vendors-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/openapi/vantaca-openapi.json
consequence_counts:
  physical: 8
  read: 44
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vantaca Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /AP/approveInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /AP/createInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /AP/deleteInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /AP/payInvoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /AP/updateInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /AP/updateInvoiceAttachment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /AP/voidInvoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /write/createWorkOrder
operation_count: 75
overview: 'Vantaca exposes 75 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 44 read, 23 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vantaca
provider_slug: vantaca
slug: vantaca-agentic-access
source_filename: vantaca-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vantaca-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 75\n  by_action_class:\n    connected: 44\n    acting: 31\n  by_consequence:\n    read: 44\n    write: 23\n    physical: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /read/ARCList\n  method: get\n  operationId: ARCList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/Association\n  method: get\n  operationId: associationList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/AssociationAddress\n\
  \  method: get\n  operationId: AssociationAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/AttachmentList\n  method: get\n  operationId: attachmentList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/getEmail\n  method: get\n  operationId: getEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/getPhone\n  method: get\n  operationId: getPhone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/getActionItem\n  method: get\n  operationId: getActionItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/getAddress\n  method: get\n  operationId: getAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/getCommPreference\n  method: get\n  operationId: getCommPreference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/provider\n  method: get\n  operationId: getProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/providerSingle\n  method: get\n  operationId: getProviderSingle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/providerTypeList\n  method: get\n  operationId: returnProviderTypeList\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/getTenantData\n  method: get\n  operationId: getTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/getDocument\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/violationList\n  method: get\n  operationId: getViolationList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/violationTypeList\n  method: get\n  operationId: getViolationTypeList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /read/workOrderList\n  method: get\n  operationId: getWorkOrderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/CollectionList\n  method: get\n  operationId: getCollectionList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/actionTypeSteps\n  method: get\n  operationId: actionTypeSteps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/homeownerTransactions\n  method: get\n  operationId: getHomeownerTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/associationDetails\n  method: get\n  operationId:\
  \ getAssociationDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/associationAdditionalInfo\n  method: get\n  operationId: getAssociationAdditionalInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/homeownerAccountInfo\n  method: get\n  operationId: getHomeownerAccountInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/homeownerAssessment\n  method: get\n  operationId: homeownerAssessment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/homeownerSearch\n  method: get\n  operationId: searchHomeowners\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/ccrItemList\n  method: get\n  operationId: getccrItemList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/glHistoryDetail\n  method: get\n  operationId: getGLHistoryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/actionCategoryList\n  method: get\n  operationId: getActionCategoryList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/actionTypeList\n  method: get\n  operationId: getActionTypeList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /write/emailCreate\n  method: post\n  operationId: createEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/emailUpdate\n  method: post\n  operationId: updateEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/emailDestroy\n  method: post\n  operationId: deleteEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /write/phoneCreate\n  method: post\n  operationId: createPhone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/phoneUpdate\n  method: post\n  operationId: updatePhone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/phoneDestroy\n  method: post\n  operationId: destroyPhone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/addressCreate\n  method: post\n  operationId: createAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/addressUpdate\n  method: post\n  operationId: updateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/addressDestroy\n  method: post\n  operationId: destroyAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/commPrefUpdate\n  method: post\n  operationId: updateCommPreference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/createProvider\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/providerUpdate\n  method: post\n  operationId: updateProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/providerInsuranceCreate\n  method: post\n  operationId: createProviderInsurance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/providerInsuranceUpdate\n  method: post\n  operationId: updateProviderInsurance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/providerInsuranceDestroy\n  method:\
  \ post\n  operationId: destroyProviderInsurance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/createLedger\n  method: post\n  operationId: createLedger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/ledgerDelete\n  method: post\n  operationId: deleteLedger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /write/nameUpdate\n  method: post\n  operationId: updateHomeowner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/createARC\n  method: post\n  operationId: createARC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/createWorkOrder\n  method: post\n  operationId: createWorkOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Write/stepActionItem\n  method: post\n  operationId: stepActionItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/createViolation\n  method: post\n  operationId: violationCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/createStandardActionItem\n  method: post\n  operationId: createStandardActionItem\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /write/CreateActionItemNote\n  method: post\n  operationId: createActionItemNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AP/associationList\n  method: get\n  operationId: getAssociationList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/providerList\n  method: get\n  operationId: getProviderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /AP/glList\n  method: get\n  operationId: getGLList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/fundList\n  method: get\n  operationId: getFundList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/bankAccountList\n  method: get\n  operationId: getBankAccountList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/bankAccountBalance\n  method: get\n  operationId: getBankAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/createInvoice\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AP/payInvoices\n  method: post\n  operationId: postPayInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AP/updateInvoice\n  method: post\n  operationId: updateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AP/voidInvoices\n  method: post\n  operationId: voidInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AP/approveInvoice\n  method: post\n  operationId: approveInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AP/deleteInvoice\n  method: post\n  operationId: deleteInvoice\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AP/listBoardInvoices\n  method: get\n  operationId: listBoardInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/getBoardInvoice\n  method: get\n  operationId: getBoardInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/listInvoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/getInvoice\n  method: get\n  operationId:\
  \ getInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/updateInvoiceAttachment\n  method: post\n  operationId: updateInvoiceAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AP/listPayments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/getPayment\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /AP/annualBankAccountBalance\n  method: get\n  operationId: getAnnualBankAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/listAssocInvoices\n  method: get\n  operationId: listAssocInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AP/glTransactionHistory\n  method: get\n  operationId: getTransactionHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantaca/refs/heads/main/agentic-access/vantaca-agentic-access.yml
summary_line: 75 operations · 31 acting
tags:
- HOA
- Community Association Management
- CAM
- Property Management
- Real Estate
- Accounting
- Workflow Automation
- Vendor Management
---
