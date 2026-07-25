---
acting_count: 0
action_class_counts:
  connected: 30
api_specs:
- filename: chembl-activity-api-openapi.yml
  format: yaml
  label: ChEMBL Activity API
  slug: chembl-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-activity-api-openapi.yml
- filename: chembl-assay-api-openapi.yml
  format: yaml
  label: ChEMBL Assay API
  slug: chembl-assay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-assay-api-openapi.yml
- filename: chembl-atc-classification-api-openapi.yml
  format: yaml
  label: ChEMBL ATC Classification API
  slug: chembl-atc-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-atc-classification-api-openapi.yml
- filename: chembl-binding-site-api-openapi.yml
  format: yaml
  label: ChEMBL Binding Site API
  slug: chembl-binding-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-binding-site-api-openapi.yml
- filename: chembl-cell-line-api-openapi.yml
  format: yaml
  label: ChEMBL Cell Line API
  slug: chembl-cell-line-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-cell-line-api-openapi.yml
- filename: chembl-compound-record-api-openapi.yml
  format: yaml
  label: ChEMBL Compound Record API
  slug: chembl-compound-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-compound-record-api-openapi.yml
- filename: chembl-document-api-openapi.yml
  format: yaml
  label: ChEMBL Document API
  slug: chembl-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-document-api-openapi.yml
- filename: chembl-drug-api-openapi.yml
  format: yaml
  label: ChEMBL Drug API
  slug: chembl-drug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-drug-api-openapi.yml
- filename: chembl-drug-indication-api-openapi.yml
  format: yaml
  label: ChEMBL Drug Indication API
  slug: chembl-drug-indication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-drug-indication-api-openapi.yml
- filename: chembl-drug-warning-api-openapi.yml
  format: yaml
  label: ChEMBL Drug Warning API
  slug: chembl-drug-warning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-drug-warning-api-openapi.yml
- filename: chembl-mechanism-api-openapi.yml
  format: yaml
  label: ChEMBL Mechanism API
  slug: chembl-mechanism-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-mechanism-api-openapi.yml
- filename: chembl-molecule-api-openapi.yml
  format: yaml
  label: ChEMBL Molecule API
  slug: chembl-molecule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-molecule-api-openapi.yml
- filename: chembl-similarity-api-openapi.yml
  format: yaml
  label: ChEMBL Similarity API
  slug: chembl-similarity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-similarity-api-openapi.yml
- filename: chembl-status-api-openapi.yml
  format: yaml
  label: ChEMBL Status API
  slug: chembl-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-status-api-openapi.yml
- filename: chembl-substructure-api-openapi.yml
  format: yaml
  label: ChEMBL Substructure API
  slug: chembl-substructure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-substructure-api-openapi.yml
- filename: chembl-target-api-openapi.yml
  format: yaml
  label: ChEMBL Target API
  slug: chembl-target-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/openapi/chembl-target-api-openapi.yml
consequence_counts:
  read: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chembl Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'ChEMBL exposes 30 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ChEMBL
provider_slug: chembl
slug: chembl-agentic-access
source_filename: chembl-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 30\n  by_consequence:\n    read: 30\n  human_in_the_loop_required: 0\noperations:\n- path: /activity\n  method: get\n  operationId: listActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity/{activity_id}\n  method: get\n  operationId: getActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity/search\n  method: get\n  operationId: searchActivities\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assay\n  method: get\n  operationId: listAssays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assay/{assay_chembl_id}\n  method: get\n  operationId: getAssay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /molecule\n  method: get\n  operationId: listMolecules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /molecule/{molecule_chembl_id}\n  method: get\n  operationId: getMolecule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /molecule/search\n  method: get\n  operationId: searchMolecules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /target\n  method: get\n  operationId: listTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /target/{target_chembl_id}\n  method: get\n  operationId: getTarget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /target/search\n  method: get\n  operationId: searchTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drug\n  method: get\n  operationId: listDrugs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drug_indication\n  method: get\n  operationId: listDrugIndications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /drug_warning\n  method: get\n  operationId: listDrugWarnings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mechanism\n  method: get\n  operationId: listMechanisms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /similarity/{smiles}/{similarity}\n  method: get\n  operationId: similaritySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /substructure/{smiles}\n  method:\
  \ get\n  operationId: substructureSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /image/{molecule_chembl_id}\n  method: get\n  operationId: getMoleculeImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atc_class\n  method: get\n  operationId: listAtcClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /binding_site\n  method: get\n  operationId: listBindingSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cell_line\n  method: get\n  operationId: listCellLines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /chembl_id_lookup\n  method: get\n  operationId: chemblIdLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /document\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compound_record\n  method: get\n  operationId: listCompoundRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /go_slim\n  method: get\n  operationId: listGoSlim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metabolism\n  method: get\n  operationId: listMetabolism\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /protein_class\n  method: get\n  operationId: listProteinClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tissue\n  method: get\n  operationId: listTissues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /xref_source\n  method: get\n  operationId: listXrefSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chembl/refs/heads/main/agentic-access/chembl-agentic-access.yml
summary_line: 30 operations
tags:
- Drug Discovery
- Bioactivity
- Molecules
- Cheminformatics
- Life Sciences
- Bioinformatics
- Pharmacology
- EMBL-EBI
---
