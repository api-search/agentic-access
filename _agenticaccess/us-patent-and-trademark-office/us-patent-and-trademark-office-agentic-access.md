---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 33
api_specs:
- filename: us-patent-and-trademark-office-bulk-datasets-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office Bulk Datasets API
  slug: us-patent-and-trademark-office-bulk-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-bulk-datasets-api-openapi.yml
- filename: us-patent-and-trademark-office-case-documents-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office Case Documents API
  slug: us-patent-and-trademark-office-case-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-case-documents-api-openapi.yml
- filename: us-patent-and-trademark-office-case-status-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office Case Status API
  slug: us-patent-and-trademark-office-case-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-case-status-api-openapi.yml
- filename: us-patent-and-trademark-office-patent-search-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office Patent Search API
  slug: us-patent-and-trademark-office-patent-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-patent-search-api-openapi.yml
- filename: us-patent-and-trademark-office-petition-decisions-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office Petition Decisions API
  slug: us-patent-and-trademark-office-petition-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-petition-decisions-api-openapi.yml
- filename: us-patent-and-trademark-office-ptab-appeals-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office PTAB Appeals API
  slug: us-patent-and-trademark-office-ptab-appeals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-ptab-appeals-api-openapi.yml
- filename: us-patent-and-trademark-office-ptab-interferences-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office PTAB Interferences API
  slug: us-patent-and-trademark-office-ptab-interferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-ptab-interferences-api-openapi.yml
- filename: us-patent-and-trademark-office-ptab-trials-decisions-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office PTAB Trials Decisions API
  slug: us-patent-and-trademark-office-ptab-trials-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-ptab-trials-decisions-api-openapi.yml
- filename: us-patent-and-trademark-office-ptab-trials-documents-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office PTAB Trials Documents API
  slug: us-patent-and-trademark-office-ptab-trials-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-ptab-trials-documents-api-openapi.yml
- filename: us-patent-and-trademark-office-ptab-trials-proceedings-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office PTAB Trials Proceedings API
  slug: us-patent-and-trademark-office-ptab-trials-proceedings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-ptab-trials-proceedings-api-openapi.yml
consequence_counts:
  read: 33
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Us Patent And Trademark Office Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 41
overview: 'US Patent and Trademark Office exposes 41 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 33 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: US Patent and Trademark Office
provider_slug: us-patent-and-trademark-office
slug: us-patent-and-trademark-office-agentic-access
source_filename: us-patent-and-trademark-office-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/uspto-open-data-portal-openapi.yml, openapi/uspto-tsdr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    acting: 8\n    connected: 33\n  by_consequence:\n    write: 8\n    read: 33\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/patent/applications/search\n  method: post\n  operationId: searchPatentApplicationsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/patent/applications/search\n\
  \  method: get\n  operationId: searchPatentApplicationsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/search/download\n  method: post\n  operationId: downloadPatentApplicationsSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/patent/applications/{applicationNumberText}\n  method: get\n  operationId: getPatentApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/meta-data\n  method: get\n  operationId: getPatentApplicationMetaData\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/adjustment\n  method: get\n  operationId: getPatentApplicationAdjustment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/assignment\n  method: get\n  operationId: getPatentApplicationAssignment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/attorney\n  method: get\n  operationId: getPatentApplicationAttorney\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/continuity\n\
  \  method: get\n  operationId: getPatentApplicationContinuity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/foreign-priority\n  method: get\n  operationId: getPatentApplicationForeignPriority\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/transactions\n  method: get\n  operationId: getPatentApplicationTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/applications/{applicationNumberText}/documents\n  method: get\n  operationId: getPatentApplicationDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/status-codes\n  method: get\n  operationId: getPatentStatusCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/products/search\n  method: get\n  operationId: searchDatasetProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets/products/{productIdentifier}\n  method: get\n  operationId: getDatasetProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/petition/decisions/search\n  method: post\n  operationId: searchPetitionDecisionsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/petition/decisions/search\n  method: get\n  operationId: searchPetitionDecisionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/petition/decisions/{petitionDecisionRecordIdentifier}\n  method: get\n  operationId: getPetitionDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/trials/proceedings/search\n  method: post\n  operationId: searchPtabProceedingsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/patent/trials/proceedings/search\n  method: get\n  operationId: searchPtabProceedingsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/trials/proceedings/{trialNumber}\n  method: get\n  operationId: getPtabProceeding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/trials/decisions/search\n  method: post\n  operationId: searchPtabDecisionsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/patent/trials/decisions/search\n  method:\
  \ get\n  operationId: searchPtabDecisionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/trials/decisions/{documentIdentifier}\n  method: get\n  operationId: getPtabDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/trials/documents/search\n  method: post\n  operationId: searchPtabDocumentsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/patent/trials/documents/search\n  method: get\n  operationId: searchPtabDocumentsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/trials/documents/{documentIdentifier}\n  method: get\n  operationId: getPtabDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/appeals/decisions/search\n  method: post\n  operationId: searchPtabAppealDecisionsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/patent/appeals/decisions/search\n  method: get\n  operationId: searchPtabAppealDecisionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/appeals/decisions/{documentIdentifier}\n\
  \  method: get\n  operationId: getPtabAppealDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/interferences/decisions/search\n  method: post\n  operationId: searchPtabInterferenceDecisionsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/patent/interferences/decisions/search\n  method: get\n  operationId: searchPtabInterferenceDecisionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/patent/interferences/decisions/{documentIdentifier}\n  method: get\n  operationId: getPtabInterferenceDecision\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/caseMultiStatus/{type}\n  method: get\n  operationId: getMultipleCaseStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casestatus/{caseid}/content.pdf\n  method: get\n  operationId: getCaseStatusPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casedocs/{caseid}/info\n  method: get\n  operationId: getCaseDocumentsInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casedocs/{caseid}/bundle\n  method: get\n  operationId: getCaseDocumentsBundle\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casedoc/{caseid}/{docid}/info\n  method: get\n  operationId: getCaseDocumentInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casedoc/{caseid}/{docid}/content.pdf\n  method: get\n  operationId: getCaseDocumentPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ts/cd/casedoc/{caseid}/{docid}/{pageid}/media\n  method: get\n  operationId: getCaseDocumentPageMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /last-update/info.json\n  method: get\n  operationId: getLastUpdateInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/agentic-access/us-patent-and-trademark-office-agentic-access.yml
summary_line: 41 operations · 8 acting
tags:
- Federal Government
- Patents
- Trademarks
- Intellectual Property
- Open Data
---
