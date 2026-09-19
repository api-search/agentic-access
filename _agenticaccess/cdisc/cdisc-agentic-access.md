---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 45
api_specs:
- filename: cdisc-adam-api-openapi.yml
  format: yaml
  label: cdisc ADaM API
  slug: cdisc-adam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-adam-api-openapi.yml
- filename: cdisc-biomedical-concepts-api-openapi.yml
  format: yaml
  label: cdisc Biomedical Concepts API
  slug: cdisc-biomedical-concepts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-biomedical-concepts-api-openapi.yml
- filename: cdisc-cdash-api-openapi.yml
  format: yaml
  label: cdisc CDASH API
  slug: cdisc-cdash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-cdash-api-openapi.yml
- filename: cdisc-products-api-openapi.yml
  format: yaml
  label: cdisc Products API
  slug: cdisc-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-products-api-openapi.yml
- filename: cdisc-sdtm-api-openapi.yml
  format: yaml
  label: cdisc SDTM API
  slug: cdisc-sdtm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-sdtm-api-openapi.yml
- filename: cdisc-terminology-api-openapi.yml
  format: yaml
  label: cdisc Terminology API
  slug: cdisc-terminology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-terminology-api-openapi.yml
- filename: cdisc-ars-api-openapi.yml
  format: yaml
  label: CDISC Analysis Results Standard (ARS) API
  slug: cdisc-analysis-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-ars-api-openapi.yml
- filename: cdisc-dataset-json-api-openapi.json
  format: json
  label: CDISC Dataset-JSON API (standard specification)
  slug: cdisc-dataset-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-dataset-json-api-openapi.json
- filename: cdisc-usdm-api-openapi.yml
  format: yaml
  label: CDISC USDM (DDF) Study Definitions API
  slug: cdisc-usdm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/openapi/cdisc-usdm-api-openapi.yml
consequence_counts:
  read: 45
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cdisc Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 59
overview: 'Cdisc exposes 59 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cdisc
provider_slug: cdisc
slug: cdisc-agentic-access
source_filename: cdisc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: generated\nsource: openapi/cdisc-adam-api-openapi.yml, openapi/cdisc-ars-api-openapi.yml, openapi/cdisc-biomedical-concepts-api-openapi.yml,\n  openapi/cdisc-cdash-api-openapi.yml, openapi/cdisc-dataset-json-api-openapi.json, openapi/cdisc-products-api-openapi.yml,\n  openapi/cdisc-sdtm-api-openapi.yml, openapi/cdisc-terminology-api-openapi.yml, openapi/cdisc-usdm-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 59\n  by_action_class:\n    connected: 45\n    acting: 14\n  by_consequence:\n    read: 45\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /mdr/adam\n  method: get\n  operationId: listAdamVersions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/adam/{version}\n  method: get\n  operationId: getAdamVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages\n  method: get\n  operationId: api.products.ars.get_packages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents\n  method: get\n  operationId: api.products.ars.get_package_reportingevents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/analysissets/{analysisset}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_analysisset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/datasubsets/{datasubset}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_datasubset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/analysisgroupings/{analysisgrouping}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_analysisgrouping\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/analysisgroupings/{analysisgrouping}/analysisgroups/{analysisgroup}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_analysisgrouping_analysisgrou\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/methods/{method}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_method\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/methods/{method}/operations/{operation}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_method_operation\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/methods/{method}/operations/{operation}/refoprels/{refoprel}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_method_operation_refoprel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/analyses/{analysis}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_analysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/analyses/{analysis}/datagroupings/{datagrouping}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_analysis_datagrouping\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/analyses/{analysis}/datagroupings/{datagrouping}/datagroups/{datagroup}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_analysis_datagrouping_datagroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/outputs/{output}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_output\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/outputs/{output}/displays/{display}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_output_display\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/categorizations/{categorization}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_categorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ars/packages/{package}/reportingevents/{reportingevent}/categorizations/{categorization}/categories/{category}\n  method: get\n  operationId: api.products.ars.get_package_reportingevent_categorization_category\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/v2/bc\n  method: get\n  operationId: listBiomedicalConcepts\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cosmos/v2/bc/{conceptId}\n  method: get\n  operationId: getBiomedicalConcept\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/cdash\n  method: get\n  operationId: listCdashVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /about\n  method: get\n  operationId: about_about_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies\n  method: get\n  operationId: studies_studies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies\n  method: post\n  operationId:\
  \ add_study_studies_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studies/{studyOID}\n  method: get\n  operationId: study_studies__studyOID__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/{studyOID}\n  method: put\n  operationId: update_study_studies__studyOID__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studies/{studyOID}\n  method: delete\n  operationId: delete_study_studies__studyOID__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studies/{studyOID}/snapshots\n  method: post\n  operationId: add_snapshot_studies__studyOID__snapshots_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studies/{studyOID}/snapshots\n  method: get\n  operationId: snapshots_studies__studyOID__snapshots_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/{studyOID}/snapshots/{snapshotID}\n  method: get\n\
  \  operationId: snapshot_studies__studyOID__snapshots__snapshotID__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/{studyOID}/snapshots/{snapshotID}\n  method: delete\n  operationId: delete_snapshot_studies__studyOID__snapshots__snapshotID__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studies/{studyOID}/snapshots/{snapshotID}/datasets/{datasetOID}\n  method: get\n  operationId: dataset_studies__studyOID__snapshots__snapshotID__datasets__datasetOID__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/{studyOID}/datasets\n\
  \  method: get\n  operationId: datasets_studies__studyOID__datasets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/{studyOID}/datasets\n  method: post\n  operationId: post_dataset_studies__studyOID__datasets_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studies/{studyOID}/datasets/{datasetOID}\n  method: get\n  operationId: dataset_studies__studyOID__datasets__datasetOID__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/{studyOID}/datasets/{datasetOID}\n  method: put\n  operationId: update_dataset_studies__studyOID__datasets__datasetOID__put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studies/{studyOID}/datasets/{datasetOID}\n  method: patch\n  operationId: append_dataset_studies__studyOID__datasets__datasetOID__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studies/{studyOID}/datasets/{datasetOID}\n  method: delete\n  operationId: delete_dataset_studies__studyOID__datasets__datasetOID__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studies/{studyOID}/datasets/{datasetOID}/$export\n  method: get\n  operationId: export_dataset_studies__studyOID__datasets__datasetOID___export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/{studyOID}/datasets/{datasetOID}/ndjson\n  method: get\n  operationId: download_dataset_stream_studies__studyOID__datasets__datasetOID__ndjson_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/{studyOID}/defines\n  method: post\n  operationId: add_define_studies__studyOID__defines_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /studies/{studyOID}/defines\n  method: get\n  operationId: defines_studies__studyOID__defines_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/{studyOID}/defines/{label}\n  method: get\n  operationId: define_studies__studyOID__defines__label__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /studies/{studyOID}/defines/{label}\n  method: put\n  operationId: update_define_studies__studyOID__defines__label__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /studies/{studyOID}/defines/{label}\n  method: delete\n  operationId: delete_define_studies__studyOID__defines__label__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mdr/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/sdtm\n  method: get\n  operationId: listSdtmVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/sdtm/{version}\n  method: get\n  operationId: getSdtmVersion\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/sdtm/{version}/classes\n  method: get\n  operationId: listSdtmClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/sdtm/{version}/datasets\n  method: get\n  operationId: listSdtmDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/sdtm/{version}/datasets/{dataset}\n  method: get\n  operationId: getSdtmDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mdr/ct\n  method: get\n  operationId: listTerminologyPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /mdr/ct/{packageDate}/codelists\n  method: get\n  operationId: listCodelists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/studyDefinitions\n  method: post\n  operationId: create_study_v3_studyDefinitions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/studyDefinitions/{studyId}\n  method: put\n  operationId: update_study_v3_studyDefinitions__studyId__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v3/studyDefinitions/{studyId}\n  method: get\n  operationId: read_full_study_v3_studyDefinitions__studyId__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/studyDefinitions/{studyId}/history\n  method: get\n  operationId: read_study_history_v3_studyDefinitions__studyId__history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/studyDesigns\n  method: get\n  operationId: search_study_design_v3_studyDesigns_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdisc/refs/heads/main/agentic-access/cdisc-agentic-access.yml
summary_line: 59 operations · 14 acting
tags:
- Clinical Trials
- Standards
- Life Sciences
- Pharma
- Healthcare
- Metadata
- Controlled Terminology
- Data Exchange
- Non-Profit
---
