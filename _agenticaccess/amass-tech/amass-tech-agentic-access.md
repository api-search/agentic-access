---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 48
api_specs:
- filename: amass-tech-cores-biomedcore-api-openapi.yml
  format: yaml
  label: Amass Cores/biomedcore API
  slug: amass-tech-cores-biomedcore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-biomedcore-api-openapi.yml
- filename: amass-tech-cores-drugcore-api-openapi.yml
  format: yaml
  label: Amass Cores/drugcore API
  slug: amass-tech-cores-drugcore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-drugcore-api-openapi.yml
- filename: amass-tech-cores-genecore-api-openapi.yml
  format: yaml
  label: Amass Cores/genecore API
  slug: amass-tech-cores-genecore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-genecore-api-openapi.yml
- filename: amass-tech-cores-patentcore-api-openapi.yml
  format: yaml
  label: Amass Cores/patentcore API
  slug: amass-tech-cores-patentcore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-patentcore-api-openapi.yml
- filename: amass-tech-cores-regulatorycore-api-openapi.yml
  format: yaml
  label: Amass Cores/regulatorycore API
  slug: amass-tech-cores-regulatorycore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-regulatorycore-api-openapi.yml
- filename: amass-tech-cores-trialcore-api-openapi.yml
  format: yaml
  label: Amass Cores/trialcore API
  slug: amass-tech-cores-trialcore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-trialcore-api-openapi.yml
- filename: amass-tech-credits-api-openapi.yml
  format: yaml
  label: Amass Credits API
  slug: amass-tech-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-credits-api-openapi.yml
consequence_counts:
  read: 48
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amass Tech Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 50
overview: 'Amass exposes 50 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 48 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amass
provider_slug: amass-tech
slug: amass-tech-agentic-access
source_filename: amass-tech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/amass-tech-openapi.json, openapi/api.amass.tech_openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    connected: 48\n    acting: 2\n  by_consequence:\n    read: 48\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/cores/biomedcore/records\n  method: get\n  operationId: searchBiomedCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/biomedcore/records/{amassId}\n  method: get\n  operationId: getBiomedCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/biomedcore/records/lookup\n  method: post\n  operationId: lookupBiomedCoreRecordsByPmidOrDoi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cores/biomedcore/changes\n  method: get\n  operationId: listBiomedCoreChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/trialcore/records\n  method: get\n  operationId: searchTrialCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/trialcore/records/{amassId}\n \
  \ method: get\n  operationId: getTrialCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/trialcore/records/lookup\n  method: post\n  operationId: lookupTrialCoreRecordsByNctId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/trialcore/changes\n  method: get\n  operationId: listTrialCoreChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/regulatorycore/records\n  method: get\n  operationId: searchRegulatoryCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/regulatorycore/records/{amassId}\n\
  \  method: get\n  operationId: getRegulatoryCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/regulatorycore/records/{amassId}/document-sections/{documentSectionId}\n  method: get\n  operationId: getRegulatoryCoreDocumentSection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/regulatorycore/records/lookup\n  method: post\n  operationId: lookupRegulatoryCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/regulatorycore/changes\n  method: get\n  operationId: listRegulatoryCoreChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/cores/drugcore/records\n  method: get\n  operationId: searchDrugCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/drugcore/records/{amassId}\n  method: get\n  operationId: getDrugCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/drugcore/records/lookup\n  method: post\n  operationId: lookupDrugCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/drugcore/changes\n  method: get\n  operationId: listDrugCoreChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/cores/genecore/records\n  method: get\n  operationId: searchGeneCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/genecore/records/{amassId}\n  method: get\n  operationId: getGeneCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/genecore/records/lookup\n  method: post\n  operationId: lookupGeneCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/genecore/changes\n  method: get\n  operationId: listGeneCoreChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/patentcore/records\n\
  \  method: get\n  operationId: searchPatentCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/patentcore/records/{amassId}\n  method: get\n  operationId: getPatentCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/patentcore/records/lookup\n  method: post\n  operationId: lookupPatentCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credits/api-credits\n  method: get\n  operationId: getApiCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/biomedcore/records\n  method: get\n  operationId:\
  \ searchBiomedCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/biomedcore/records/{amassId}\n  method: get\n  operationId: getBiomedCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/biomedcore/records/lookup\n  method: post\n  operationId: lookupBiomedCoreRecordsByPmidOrDoi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cores/biomedcore/changes\n  method: get\n  operationId: listBiomedCoreChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/trialcore/records\n  method: get\n  operationId: searchTrialCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/trialcore/records/{amassId}\n  method: get\n  operationId: getTrialCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/trialcore/records/lookup\n  method: post\n  operationId: lookupTrialCoreRecordsByNctId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/trialcore/changes\n  method: get\n  operationId: listTrialCoreChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/regulatorycore/records\n  method: get\n  operationId: searchRegulatoryCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/regulatorycore/records/{amassId}\n  method: get\n  operationId: getRegulatoryCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/regulatorycore/records/{amassId}/document-sections/{documentSectionId}\n  method: get\n  operationId: getRegulatoryCoreDocumentSection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/regulatorycore/records/lookup\n  method: post\n  operationId: lookupRegulatoryCoreRecords\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/regulatorycore/changes\n  method: get\n  operationId: listRegulatoryCoreChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/drugcore/records\n  method: get\n  operationId: searchDrugCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/drugcore/records/{amassId}\n  method: get\n  operationId: getDrugCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/drugcore/records/lookup\n  method: post\n  operationId: lookupDrugCoreRecords\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/drugcore/changes\n  method: get\n  operationId: listDrugCoreChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/genecore/records\n  method: get\n  operationId: searchGeneCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/genecore/records/{amassId}\n  method: get\n  operationId: getGeneCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/genecore/records/lookup\n  method: post\n  operationId: lookupGeneCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/genecore/changes\n  method: get\n  operationId: listGeneCoreChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/patentcore/records\n  method: get\n  operationId: searchPatentCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/patentcore/records/{amassId}\n  method: get\n  operationId: getPatentCoreRecordByAmassId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cores/patentcore/records/lookup\n  method: post\n  operationId: lookupPatentCoreRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credits/api-credits\n  method: get\n  operationId: getApiCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/amass-tech/agentic-access/amass-tech-agentic-access.yml
summary_line: 50 operations · 2 acting
tags:
- Company
- Life Sciences
- Data Intelligence
- MCP
---
