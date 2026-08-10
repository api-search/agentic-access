---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 24
api_specs:
- filename: canoe-intelligence-allocations-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Allocations API
  slug: canoe-intelligence-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-allocations-api-openapi.yml
- filename: canoe-intelligence-authentication-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Authentication API
  slug: canoe-intelligence-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-authentication-api-openapi.yml
- filename: canoe-intelligence-custom-fields-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Custom Fields API
  slug: canoe-intelligence-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-custom-fields-api-openapi.yml
- filename: canoe-intelligence-documents-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Documents API
  slug: canoe-intelligence-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-documents-api-openapi.yml
- filename: canoe-intelligence-funds-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Funds API
  slug: canoe-intelligence-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-funds-api-openapi.yml
- filename: canoe-intelligence-organizations-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Organizations API
  slug: canoe-intelligence-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-organizations-api-openapi.yml
- filename: canoe-intelligence-password-grant-tokens-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Password Grant Tokens API
  slug: canoe-intelligence-password-grant-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-password-grant-tokens-api-openapi.yml
- filename: canoe-intelligence-terms-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Terms API
  slug: canoe-intelligence-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-terms-api-openapi.yml
- filename: canoe-intelligence-user-api-openapi.yml
  format: yaml
  label: Canoe Intelligence User API
  slug: canoe-intelligence-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-user-api-openapi.yml
consequence_counts:
  read: 24
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Canoe Intelligence Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 50
overview: 'Canoe Intelligence exposes 50 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 26 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Canoe Intelligence
provider_slug: canoe-intelligence
slug: canoe-intelligence-agentic-access
source_filename: canoe-intelligence-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/canoe-intelligence-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    connected: 24\n    acting: 26\n  by_consequence:\n    read: 24\n    write: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/allocations\n  method: get\n  operationId: GetAllocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/allocations\n  method: post\n  operationId: CreateSingleAllocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/allocations/{id}\n  method: put\n  operationId: UpdateSingleAllocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/allocations/{id}\n  method: delete\n  operationId: DeleteSingleAllocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/data\n  method: get\n  operationId: GetDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/types\n  method: get\n  operationId: GetDocumentsType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/tags\n  method: get\n  operationId: GetDocumentTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/allocation-tags\n  method: get\n  operationId: GetDocumentAllocationTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/delete-documents\n  method: post\n  operationId: DeleteMultipleDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{id}\n  method: get\n  operationId: GetASingleDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents/{id}\n  method: delete\n  operationId: DeleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/metadata\n  method: post\n  operationId: BulkSetDocumentMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{id}/metadata\n  method: put\n  operationId: SetDocumentMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents\n  method: get\n  operationId: DownloadDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/documents\n  method: post\n  operationId: UploadDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/funds\n\
  \  method: get\n  operationId: GetFunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/funds\n  method: post\n  operationId: CreateSingleFund\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/funds\n  method: delete\n  operationId: DeleteMultipleFunds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/funds/details\n  method: get\n  operationId: GetFundsDetailedData\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/funds/{id}\n  method: get\n  operationId: GetSingleFunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/funds/{id}\n  method: put\n  operationId: UpdateSingleFund\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/funds/{id}\n  method: delete\n  operationId: DeleteSingleFund\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/funds/{id}/document-data\n  method: get\n  operationId: GetSingleFundsDocumentdata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/funds/{id}/documents\n  method: get\n  operationId: DownloadSingleFundsDocumentdata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/funds/{id}/document-ids\n  method: get\n  operationId: GetSingleFundsDocumentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations\n  method: get\n  operationId: Organizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{id}\n  method:\
  \ get\n  operationId: FindById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{id}/document-data\n  method: get\n  operationId: FindBySingleOrganizationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{id}/documents\n  method: get\n  operationId: DownloadOrganizationDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{id}/document-ids\n  method: get\n  operationId: DownloadBySingleOrganizationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/entities\n  method: post\n  operationId: CreateASingleEntity\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/entities/{id}\n  method: put\n  operationId: UpdateASingleEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/accounts\n  method: post\n  operationId: CreateASingleAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/organizations/accounts/{id}\n  method: put\n  operationId: UpdateASingleAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/custom_fields\n  method: get\n  operationId: GetCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user\n  method: get\n  operationId: User\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users\n  method: get\n  operationId: findByTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tokens\n  method: post\n  operationId: Tokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/clients\n  method: get\n  operationId: ManageAuthClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n  operationId: RequestingTokensAuthCodes\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token/refresh\n  method: post\n  operationId: RequestingTokensRefreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token/client-credentials\n  method: post\n  operationId: RequestingTokensClientCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/terms\n  method: get\n  operationId: GetTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/terms\n  method: post\n  operationId: CreateSingleTerm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/terms/{id}\n  method: put\n  operationId: UpdateSingleTerm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/terms/{id}\n  method: delete\n  operationId: DeleteSingleTerm\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/documents/{allocationId}/allocation-tags\n  method: patch\n  operationId: updateAllocationTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{id}\n  method: put\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/roles\n  method:\
  \ get\n  operationId: getUserRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/agentic-access/canoe-intelligence-agentic-access.yml
summary_line: 50 operations · 26 acting
tags:
- alternative-investments
- private-markets
- document-automation
- data-extraction
- fund-administration
- capital-calls
- k-1-tax-documents
- portfolio-reporting
- financial-services
- fintech
- wealth-management
- institutional-investors
---
