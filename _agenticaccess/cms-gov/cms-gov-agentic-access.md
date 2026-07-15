---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 57
api_specs:
- filename: cms-gov-blue-button-2-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 API
  slug: blue-button-2-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-blue-button-2-openapi.yml
- filename: cms-gov-bcda-openapi.yml
  format: yaml
  label: CMS Beneficiary Claims Data API (BCDA)
  slug: beneficiary-claims-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-bcda-openapi.yml
- filename: cms-gov-ab2d-openapi.yml
  format: yaml
  label: CMS AB2D API
  slug: ab2d-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-ab2d-openapi.yml
- filename: cms-gov-dpc-openapi.yml
  format: yaml
  label: CMS Data at the Point of Care API (DPC)
  slug: data-at-point-of-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-dpc-openapi.yml
- filename: cms-gov-bfd-openapi.yml
  format: yaml
  label: CMS Beneficiary FHIR Data Server (BFD)
  slug: bfd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-bfd-openapi.yml
- filename: cms-gov-marketplace-openapi.yml
  format: yaml
  label: CMS Marketplace API
  slug: marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-marketplace-openapi.yml
- filename: cms-gov-open-data-openapi.yml
  format: yaml
  label: CMS Open Data API (data.cms.gov)
  slug: data-cms-gov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-open-data-openapi.yml
- filename: cms-gov-provider-data-openapi.yml
  format: yaml
  label: CMS Provider Data Catalog API
  slug: provider-data-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-provider-data-openapi.yml
- filename: cms-gov-qpp-openapi.yml
  format: yaml
  label: CMS Quality Payment Program API
  slug: quality-payment-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-qpp-openapi.yml
- filename: cms-gov-mcd-openapi.yml
  format: yaml
  label: CMS Medicare Coverage Database API
  slug: medicare-coverage-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-mcd-openapi.yml
consequence_counts:
  read: 57
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cms Gov Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 71
overview: 'CMS — Centers for Medicare & Medicaid Services exposes 71 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 57 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CMS — Centers for Medicare & Medicaid Services
provider_slug: cms-gov
slug: cms-gov-agentic-access
source_filename: cms-gov-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cms-gov-ab2d-openapi.yml, openapi/cms-gov-bcda-openapi.yml, openapi/cms-gov-bfd-openapi.yml,\n  openapi/cms-gov-blue-button-2-openapi.yml, openapi/cms-gov-dpc-openapi.yml, openapi/cms-gov-marketplace-openapi.yml,\n  openapi/cms-gov-mcd-openapi.yml, openapi/cms-gov-open-data-openapi.yml, openapi/cms-gov-provider-data-openapi.yml,\n  openapi/cms-gov-qpp-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 71\n  by_action_class:\n    connected: 57\n    acting: 14\n  by_consequence:\n    read: 57\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /Patient/$export\n  method: get\n  operationId: exportPatient\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Group/{contractId}/$export\n  method: get\n  operationId: exportContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Job/{jobUuid}/$status\n  method: get\n  operationId: getJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Job/{jobUuid}/$status\n  method: delete\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Job/{jobUuid}/file/{filename}\n  method: get\n  operationId: downloadOutput\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/$export\n  method: get\n  operationId: exportPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Group/{groupId}/$export\n  method: get\n  operationId: exportGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /jobs/{jobId}\n  method: delete\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attribution_status\n  method: get\n  operationId: getAttributionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient\n\
  \  method: get\n  operationId: searchPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}\n  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Coverage\n  method: get\n  operationId: searchCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ExplanationOfBenefit\n  method: get\n  operationId: searchExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Group/{id}/$export\n  method: get\n  operationId: exportGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /Patient\n  method: get\n  operationId: searchPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /Patient/{id}\n  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /Coverage\n  method: get\n  operationId: searchCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n  \
  \  - read\n- path: /Coverage/{id}\n  method: get\n  operationId: readCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /ExplanationOfBenefit\n  method: get\n  operationId: searchExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /ExplanationOfBenefit/{id}\n  method: get\n  operationId: readExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /userinfo\n  method: get\n  operationId: getUserinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n\
  - path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organization\n  method: get\n  operationId: searchOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organization/{id}\n  method: get\n  operationId: readOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Practitioner\n  method: post\n  operationId: createPractitioner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /Practitioner\n  method: get\n  operationId: searchPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Practitioner/{id}\n  method: get\n  operationId: readPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Practitioner/{id}\n  method: delete\n  operationId: deletePractitioner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Patient\n  method: post\n  operationId: createPatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Patient\n  method: get\n  operationId: searchPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Group\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Group/{groupId}\n  method: get\n  operationId: readGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Group/{groupId}\n  method: put\n  operationId: updateGroup\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Group/{groupId}/$export\n  method: get\n  operationId: exportGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Jobs/{jobId}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Data/{fileName}\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/search\n  method: post\n  operationId: searchPlans\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans/{planId}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counties/by/zip/{zip}\n  method: get\n  operationId: getCountiesByZip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /issuers\n  method: get\n  operationId: listIssuers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/search\n  method: post\n  operationId: searchProviders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /drugs/autocomplete\n  method: get\n  operationId: drugAutocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/eligibility\n  method: post\n  operationId: checkEligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ncds\n  method: get\n  operationId: searchNCDs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ncds/{ncdId}\n  method: get\n  operationId: getNCD\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lcds\n  method: get\n  operationId: searchLCDs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lcds/{lcdId}\n  method: get\n  operationId: getLCD\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles\n  method:\
  \ get\n  operationId: searchArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /medcac\n  method: get\n  operationId: searchMedcac\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataset\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataset/{datasetId}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataset/{datasetId}/data\n  method: get\n  operationId: getDatasetData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /dataset/{datasetId}/data-stats\n  method: get\n  operationId: getDatasetStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metastore/schemas/dataset/items\n  method: get\n  operationId: listProviderDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metastore/schemas/dataset/items/{datasetId}\n  method: get\n  operationId: getProviderDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datastore/query/{distributionId}\n  method: get\n  operationId: queryDistribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /datastore/sql\n  method: get\n  operationId: runSql\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions\n  method: get\n  operationId: listSubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions\n  method: post\n  operationId: createSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submissions/{id}\n  method: get\n  operationId: getSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions/{id}\n\
  \  method: put\n  operationId: updateSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /measurements\n  method: get\n  operationId: listMeasurements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /measurements\n  method: post\n  operationId: createMeasurement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scoring\n  method: get\n  operationId: getScore\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /benchmarks\n  method: get\n  operationId: listBenchmarks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/agentic-access/cms-gov-agentic-access.yml
summary_line: 71 operations · 14 acting
tags:
- Healthcare
- Medicare
- Medicaid
- FHIR
- Bulk Data
- Open Data
- Government
- Federal
- Claims
- Insurance
- ACA
- Marketplace
- Quality
---
