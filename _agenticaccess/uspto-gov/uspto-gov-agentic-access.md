---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 47
api_specs:
- filename: uspto-gov-appeals-api-openapi.yml
  format: yaml
  label: USPTO Appeals API
  slug: uspto-gov-appeals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-appeals-api-openapi.yml
- filename: uspto-gov-application-api-openapi.yml
  format: yaml
  label: USPTO Application API
  slug: uspto-gov-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-application-api-openapi.yml
- filename: uspto-gov-assignments-api-openapi.yml
  format: yaml
  label: USPTO Assignments API
  slug: uspto-gov-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-assignments-api-openapi.yml
- filename: uspto-gov-citations-api-openapi.yml
  format: yaml
  label: USPTO Citations API
  slug: uspto-gov-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-citations-api-openapi.yml
- filename: uspto-gov-datasets-api-openapi.yml
  format: yaml
  label: USPTO Datasets API
  slug: uspto-gov-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-datasets-api-openapi.yml
- filename: uspto-gov-decisions-api-openapi.yml
  format: yaml
  label: USPTO Decisions API
  slug: uspto-gov-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-decisions-api-openapi.yml
- filename: uspto-gov-documents-api-openapi.yml
  format: yaml
  label: USPTO Documents API
  slug: uspto-gov-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-documents-api-openapi.yml
- filename: uspto-gov-enriched-citations-api-openapi.yml
  format: yaml
  label: USPTO Enriched Citations API
  slug: uspto-gov-enriched-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-enriched-citations-api-openapi.yml
- filename: uspto-gov-office-actions-api-openapi.yml
  format: yaml
  label: USPTO Office Actions API
  slug: uspto-gov-office-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-office-actions-api-openapi.yml
- filename: uspto-gov-patentsview-api-openapi.yml
  format: yaml
  label: USPTO Patentsview API
  slug: uspto-gov-patentsview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-patentsview-api-openapi.yml
- filename: uspto-gov-proceedings-api-openapi.yml
  format: yaml
  label: USPTO Proceedings API
  slug: uspto-gov-proceedings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-proceedings-api-openapi.yml
- filename: uspto-gov-rejections-api-openapi.yml
  format: yaml
  label: USPTO Rejections API
  slug: uspto-gov-rejections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-rejections-api-openapi.yml
- filename: uspto-gov-search-api-openapi.yml
  format: yaml
  label: USPTO Search API
  slug: uspto-gov-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-search-api-openapi.yml
- filename: uspto-gov-status-api-openapi.yml
  format: yaml
  label: USPTO Status API
  slug: uspto-gov-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-gov-status-api-openapi.yml
consequence_counts:
  read: 47
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Uspto Gov Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 48
overview: 'USPTO exposes 48 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 47 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: USPTO
provider_slug: uspto-gov
slug: uspto-gov-agentic-access
source_filename: uspto-gov-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/uspto-bulk-data-openapi.yml, openapi/uspto-office-actions-openapi.yml, openapi/uspto-patent-file-wrapper-openapi.yml,\n  openapi/uspto-patentsview-openapi.yml, openapi/uspto-ptab-openapi.yml, openapi/uspto-tsdr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 47\n    acting: 1\n  by_consequence:\n    read: 47\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/datasets/products/search\n  method: get\n  operationId: searchBulkProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/products/{productIdentifier}\n\
  \  method: get\n  operationId: getBulkProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/products/{productIdentifier}/files/{fileName}\n  method: get\n  operationId: downloadBulkProductFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oa/text/search\n  method: get\n  operationId: searchOfficeActionText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oa/text/{officeActionIdentifier}\n  method: get\n  operationId: getOfficeActionText\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oa/citations/search\n  method: get\n  operationId:\
  \ searchOfficeActionCitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oa/citations/fields\n  method: get\n  operationId: getOfficeActionCitationFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oa/rejections/search\n  method: get\n  operationId: searchOfficeActionRejections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oa/rejections/fields\n  method: get\n  operationId: getOfficeActionRejectionFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oa/enriched-citations/search\n  method: get\n  operationId: searchEnrichedCitations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oa/enriched-citations/fields\n  method: get\n  operationId: getEnrichedCitationFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/search\n  method: get\n  operationId: searchPatentApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/search\n  method: post\n  operationId: searchPatentApplicationsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/patent/applications/{applicationNumberText}\n  method: get\n  operationId: getPatentApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/meta-data\n  method: get\n  operationId: getPatentApplicationMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/adjustment\n  method: get\n  operationId: getPatentTermAdjustment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/assignment\n  method: get\n  operationId: getPatentAssignments\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/attorney\n  method: get\n  operationId: getApplicationAttorney\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/continuity\n  method: get\n  operationId: getApplicationContinuity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/foreign-priority\n  method: get\n  operationId: getApplicationForeignPriority\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/transactions\n\
  \  method: get\n  operationId: getApplicationTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/documents\n  method: get\n  operationId: listApplicationDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/download/applications/{applicationNumberText}/{documentId}.pdf\n  method: get\n  operationId: downloadApplicationDocumentPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patentsview/patents\n  method: get\n  operationId: queryPatents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/patentsview/inventors\n  method: get\n  operationId: queryInventors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patentsview/assignees\n  method: get\n  operationId: queryAssignees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patentsview/locations\n  method: get\n  operationId: queryLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patentsview/cpc_subsections\n  method: get\n  operationId: queryCpcSubsections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ptab/proceedings/search\n  method: get\n  operationId:\
  \ searchPtabProceedings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ptab/proceedings/{proceedingNumber}\n  method: get\n  operationId: getPtabProceeding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ptab/decisions/search\n  method: get\n  operationId: searchPtabDecisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ptab/decisions/{decisionIdentifier}\n  method: get\n  operationId: getPtabDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ptab/documents/search\n  method: get\n  operationId: searchPtabDocuments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ptab/documents/{documentIdentifier}\n  method: get\n  operationId: getPtabDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ptab/documents/{documentIdentifier}/download\n  method: get\n  operationId: downloadPtabDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ptab/appeals/search\n  method: get\n  operationId: searchPtabAppeals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ptab/interferences/search\n  method: get\n  operationId: searchPtabInterferences\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casestatus/sn{serialNumber}/info.xml\n  method: get\n  operationId: getCaseStatusBySerialNumberXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casestatus/sn{serialNumber}/info.json\n  method: get\n  operationId: getCaseStatusBySerialNumberJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casestatus/rn{registrationNumber}/info.xml\n  method: get\n  operationId: getCaseStatusByRegistrationNumberXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casestatus/rn{registrationNumber}/info.json\n  method: get\n  operationId: getCaseStatusByRegistrationNumberJson\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casestatus/rf{referenceNumber}/info.xml\n  method: get\n  operationId: getCaseStatusByReferenceNumberXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casestatus/ir{internationalRegistrationNumber}/info.xml\n  method: get\n  operationId: getCaseStatusByIrNumberXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casestatus/sn{serialNumber}/info.st96.xml\n  method: get\n  operationId: getCaseStatusBySerialNumberSt96\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casedocs/bundle.pdf\n  method:\
  \ get\n  operationId: getCaseDocumentsPdfBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casedocs/bundle.zip\n  method: get\n  operationId: getCaseDocumentsZipBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casedocs/{sn}/{documentIdentifier}.pdf\n  method: get\n  operationId: getCaseDocumentPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/rgbimg/sn{serialNumber}/{imageType}.jpg\n  method: get\n  operationId: getMarkImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/agentic-access/uspto-gov-agentic-access.yml
summary_line: 48 operations · 1 acting
tags:
- Patents
- Trademarks
- Intellectual Property
- Government
- Federal
- Open Data
- PTAB
- TSDR
---
