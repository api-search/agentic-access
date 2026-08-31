---
acting_count: 1656
action_class_counts:
  acting: 1656
  connected: 1684
api_specs:
- filename: sertica-web-api-openapi.json
  format: json
  label: SERTICA Web API
  slug: sertica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sertica/refs/heads/main/openapi/sertica-web-api-openapi.json
consequence_counts:
  physical: 167
  read: 1684
  safety-critical: 26
  write: 1463
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 26
kind: agentic-access
layout: agentic-access
method: generated
name: Sertica Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /Auth/resetPassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /Auth/resetPin
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /Auth/totp/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /Components/{componentNo}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /Components/{componentNo}/resetcounter
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ControlledCopies
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ControlledCopies/search
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ControlledCopies/searchCount
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ControlledCopies/searchIndex/{controlledCopyGuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /ControlledCopies/{copyNo}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /ControlledCopies/{copyNo}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ControlledCopies/{copyNo}/email
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ControlledCopyRevisionDocuments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ControlledCopyRevisionDocuments/search
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ControlledCopyRevisionDocuments/searchCount
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ControlledCopyRevisionDocuments/searchIndex/{documentGuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /ControlledCopyRevisionDocuments/{documentNo}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /ControlledCopyRevisionDocuments/{documentNo}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ControlledCopyRevisionDocuments/{documentNo}/checkin
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /ControlledCopyRevisionDocuments/{documentNo}/checkout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ControlledCopyRevisionDocuments/{documentNo}/file
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /IosDataSync/ResetObjectIosDataSync
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /Jobs/{jobNo}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /Options/defaultreportLogo
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /UserRights/{userRightKey}/{userGroupNo}
operation_count: 3340
overview: 'SERTICA exposes 3340 API operations that an AI agent could call, of which 1656 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1684 read, 1463 write, 167 physical, and 26 safety-critical.


  26 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SERTICA
provider_slug: sertica
slug: sertica-agentic-access
source_filename: sertica-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: generated\nsource: openapi/sertica-web-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3340\n  by_action_class:\n    connected: 1684\n    acting: 1656\n  by_consequence:\n    read: 1684\n    write: 1463\n    physical: 167\n    safety-critical: 26\n  human_in_the_loop_required: 26\noperations:\n- path: /AccountingDimensions\n  method: get\n  operationId: GetAccountingDimensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensions\n  method: post\n  operationId: CreateAccountingDimension\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AccountingDimensions/{dimensionNo}\n  method: get\n  operationId: GetAccountingDimension\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensions/{dimensionNo}\n  method: put\n  operationId: UpdateAccountingDimension\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AccountingDimensions/{dimensionNo}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AccountingDimensions/{dimensionNo}/history\n  method: get\n  operationId: GetAccountingDimensionHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensions/search\n  method: post\n  operationId: SearchAccountingDimensions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AccountingDimensions/searchCount\n  method: post\n  operationId: SearchCountAccountingDimensions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AccountingDimensions/searchIndex/{accountingDimensionGuid}\n  method: post\n  operationId: SearchIndexAccountingDimensions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AccountingDimensions/searchInfo\n  method: get\n  operationId: SearchInfoAccountingDimensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensions/{dimensionNo}/copy\n  method: get\n  operationId: CopyAccountingDimension\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensions/{dimensionNo}/values\n  method: get\n  operationId: GetAccountingDimensionValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensions/{dimensionNo}/derivedvalues\n  method: get\n  operationId: GetAccountingDimensionDerivedValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensions/{dimensionNo}/mandatoryvalues\n  method: get\n  operationId: GetAccountingDimensionMandatoryValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensions/{dimensionNo}/affectors\n  method: get\n  operationId: GetAccountingDimensionAccountingDimensionAffectors\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensionsCache/affectors\n  method: get\n  operationId: GetAccountingDimensionAffectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensionsCache/affectors/search\n  method: post\n  operationId: SearchAccountingDimensionAffectors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AccountingDimensionsCache/affectors/searchInfo\n  method: get\n  operationId: SearchInfoAccountingDimensionAffectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensionsCache/affectors/searchCount\n  method: post\n  operationId: SearchCountAccountingDimensionAffectors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AccountingDimensionsCache/affectors/{affectorGuid}/values\n  method: get\n  operationId: GetAffectorValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountingDimensionsCache/affectors/{affectorGuid}/values/search\n  method: post\n  operationId: SearchAffectorValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AccountingDimensionsCache/availableValues/{objectType}\n  method: post\n  operationId: GetAvailableValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Accounts\n  method: get\n  operationId: GetAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Accounts\n  method: post\n  operationId: CreateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Accounts/{accountNo}\n  method: get\n  operationId: GetAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Accounts/{accountNo}\n  method: put\n  operationId: UpdateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Accounts/{accountNo}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Accounts/{accountNo}/history\n\
  \  method: get\n  operationId: GetAccountHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Accounts/search\n  method: post\n  operationId: SearchAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Accounts/searchIndex/{accountGuid}\n  method: post\n  operationId: SearchIndexAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Accounts/searchCount\n  method: post\n  operationId: SearchCountAccounts\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Accounts/searchInfo\n  method: get\n  operationId: SearchInfoAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Accounts/{accountNo}/copy\n  method: get\n  operationId: CopyAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ActivityGroups\n  method: get\n  operationId: GetActivityGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ActivityGroups\n  method: post\n  operationId:\
  \ CreateActivityGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ActivityGroups/{activityGroupNo}\n  method: get\n  operationId: GetActivityGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ActivityGroups/{activityGroupNo}\n  method: put\n  operationId: UpdateActivityGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ActivityGroups/{activityGroupNo}\n  method: delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ActivityGroups/{activityGroupNo}/history\n  method: get\n  operationId: GetActivityGroupHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ActivityGroups/search\n  method: post\n  operationId: SearchActivityGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ActivityGroups/searchIndex/{activityGroupGuid}\n  method: post\n  operationId: SearchIndexActivityGroups\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ActivityGroups/searchCount\n  method: post\n  operationId: SearchCountActivityGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ActivityGroups/searchInfo\n  method: get\n  operationId: SearchInfoActivityGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ActivityGroups/{activityGroupNo}/copy\n  method: get\n  operationId: CopyActivityGroup\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AddressCategories\n  method: get\n  operationId: AddressCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AddressCategories\n  method: post\n  operationId: CreateAddressCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressCategories/{addressCategoryNo}\n  method: get\n  operationId: GetAddressCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AddressCategories/{addressCategoryNo}\n  method: put\n  operationId: UpdateAddressCategory\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressCategories/{addressCategoryNo}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressCategories/{addressCategoryNo}/history\n  method: get\n  operationId: GetAddressCategoryHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AddressCategories/search\n  method: post\n  operationId: SearchAddressCategories\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressCategories/searchIndex/{addressCategoryGuid}\n  method: post\n  operationId: SearchIndexAddressCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressCategories/searchCount\n  method: post\n  operationId: SearchCountAddressCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /AddressCategories/searchInfo\n  method: get\n  operationId: SearchInfoAddressCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AddressCategories/{addressCategoryNo}/copy\n  method: get\n  operationId: CopyAddressCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AddressClassifications\n  method: get\n  operationId: GetAddressClassifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AddressClassifications\n  method: post\n  operationId: CreateAddressClassification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressClassifications/{classificationNo}\n  method: get\n  operationId: GetAddressClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AddressClassifications/{classificationNo}\n  method: put\n  operationId: UpdateAddressClassification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressClassifications/{classificationNo}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressClassifications/{classificationNo}/history\n  method: get\n  operationId: GetAddressClassificationHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AddressClassifications/search\n  method: post\n  operationId: SearchAddressClassifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressClassifications/searchIndex/{addressClassificationGuid}\n  method: post\n  operationId: SearchIndexAddressClassifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressClassifications/searchCount\n  method: post\n  operationId: SearchCountAddressClassifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddressClassifications/searchInfo\n  method: get\n  operationId: SearchInfoAddressClassifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AddressClassifications/{classificationNo}/copy\n  method: get\n  operationId: CopyAddressClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses\n  method: get\n  operationId: GetAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses\n  method: post\n  operationId: CreateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Addresses/{addressNo}\n  method: get\n  operationId: GetAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}\n  method: put\n  operationId: UpdateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Addresses/{addressNo}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Addresses/{addressNo}/history\n  method: get\n  operationId: GetAddressHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/search\n  method: post\n  operationId: SearchAddresses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Addresses/searchCount\n  method: post\n  operationId: SearchCountAddresss\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Addresses/searchIndex/{addressGuid}\n  method: post\n  operationId: SearchIndexAddresses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Addresses/searchInfo\n  method: get\n  operationId: SearchInfoAddresss\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}/Contacts\n  method: get\n  operationId: GetAddressContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}/AddressEvaluations\n  method: get\n  operationId: GetAddressEvaluations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/addressEvaluations/{groupId}\n  method: get\n  operationId: GetAddressEvaluationsByGroupId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/addressEvaluations\n  method: post\n  operationId: CreateAddressEvaluations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Addresses/addressEvaluations\n  method: put\n  operationId: UpdateAddressEvaluations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Addresses/searchAddressEvaluations\n  method: post\n  operationId: SearchAddressEvaluations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Addresses/{addressNo}/Documents\n  method: get\n  operationId: GetAddressDocumentLinks\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}/copy\n  method: get\n  operationId: CopyAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}/responses\n  method: get\n  operationId: GetAddressResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}/responses/count\n  method: get\n  operationId: CountAddressResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{AddressNo}/addResponse\n  method: post\n  operationId: AddAddressResponse\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Addresses/{addressNo}/units\n  method: get\n  operationId: GetAddressUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}/itemtypes\n  method: get\n  operationId: GetAddressItemTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}/addressaddresscategories\n  method: get\n  operationId: GetAddressAddressCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}/deliverycosts\n\
  \  method: get\n  operationId: GetAddressDeliveryCosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}/alternatepayers\n  method: get\n  operationId: GetAddressAlternatePayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}/punchouts\n  method: get\n  operationId: GetAddressPunchOuts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Addresses/{addressNo}/contacts/{guid}/generateConnectPassword\n  method: post\n  operationId: GenerateAddressContactConnectPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Addresses/{addressNo}/contacts/{guid}/unlockAccount\n  method: post\n  operationId: UnlockAddressContactAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AiClient/ask-question\n  method: put\n  operationId: AIAskQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Analytics\n  method: get\n  operationId: GetAllMenuItems\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Analytics\n  method: post\n  operationId: CreateReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Analytics/{reportNo}\n  method: get\n  operationId: GetAnalyticsReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Analytics/{reportNo}\n  method: put\n  operationId: UpdateReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /Analytics/{reportNo}\n  method: delete\n  operationId: DeleteReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Analytics/{reportNo}/copy\n  method: get\n  operationId: CopyReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Analytics/{reportNo}/outputFields\n  method: get\n  operationId: GetReportOutputFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Analytics/{reportNo}/filterFields\n  method: get\n  operationId: GetReportFilterFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Analytics/{reportNo}/excel\n  method: get\n  operationId: GetReportExcelByNo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Analytics/excel\n  method: post\n  operationId: GetReportExcel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Analytics/reportSetting/{settingsKey}/excel\n  method: get\n  operationId: GetReportExcelByUserSetting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Analytics/{reportNo}/dataset\n  method: get\n  operationId: GetReportDatasetByNo\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Analytics/dataset\n  method: post\n  operationId: GetReportDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Analytics/reportSetting/{settingsKey}/dataset\n  method: get\n  operationId: GetReportDatasetByUserSetting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Analytics/{templateFieldName}/distinctList/{filtered}\n  method: post\n  operationId: GetDistinctList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditio\n\n# --- truncated at 32 KB (977 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/sertica/refs/heads/main/agentic-access/sertica-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sertica/refs/heads/main/agentic-access/sertica-agentic-access.yml
summary_line: 3340 operations · 1656 acting · 26 human-in-the-loop
tags:
- Maritime
- Shipping
- Fleet Management
- Maintenance
- Procurement
- Asset Management
- Compliance
- Enterprise Software
---
