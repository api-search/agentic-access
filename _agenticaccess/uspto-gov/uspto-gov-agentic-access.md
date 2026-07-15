---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 47
api_specs:
- filename: uspto-patent-file-wrapper-openapi.yml
  format: yaml
  label: USPTO Patent File Wrapper API
  slug: uspto-patent-file-wrapper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-patent-file-wrapper-openapi.yml
- filename: uspto-ptab-openapi.yml
  format: yaml
  label: USPTO Patent Trial and Appeal Board (PTAB) API
  slug: uspto-ptab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-ptab-openapi.yml
- filename: uspto-tsdr-openapi.yml
  format: yaml
  label: USPTO Trademark Status and Document Retrieval (TSDR) API
  slug: uspto-tsdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-tsdr-openapi.yml
- filename: uspto-office-actions-openapi.yml
  format: yaml
  label: USPTO Office Action APIs
  slug: uspto-office-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-office-actions-openapi.yml
- filename: uspto-bulk-data-openapi.yml
  format: yaml
  label: USPTO Bulk Data Storage System (BDSS) API
  slug: uspto-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-bulk-data-openapi.yml
- filename: uspto-patentsview-openapi.yml
  format: yaml
  label: USPTO PatentsView API
  slug: patentsview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto-gov/refs/heads/main/openapi/uspto-patentsview-openapi.yml
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
