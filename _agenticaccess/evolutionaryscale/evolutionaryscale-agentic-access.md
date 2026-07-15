---
acting_count: 11
action_class_counts:
  acting: 11
api_specs:
- filename: evolutionaryscale-forge-esm3-api-openapi.yml
  format: yaml
  label: EvolutionaryScale Forge ESM3 API
  slug: forge-esm3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/openapi/evolutionaryscale-forge-esm3-api-openapi.yml
- filename: evolutionaryscale-forge-esmc-api-openapi.yml
  format: yaml
  label: EvolutionaryScale Forge ESM Cambrian API
  slug: forge-esmc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/openapi/evolutionaryscale-forge-esmc-api-openapi.yml
- filename: evolutionaryscale-forge-folding-api-openapi.yml
  format: yaml
  label: EvolutionaryScale Forge Folding API
  slug: forge-folding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/openapi/evolutionaryscale-forge-folding-api-openapi.yml
consequence_counts:
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Evolutionaryscale Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'EvolutionaryScale exposes 11 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: EvolutionaryScale
provider_slug: evolutionaryscale
slug: evolutionaryscale-agentic-access
source_filename: evolutionaryscale-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/evolutionaryscale-forge-esm3-api-openapi.yml, openapi/evolutionaryscale-forge-esmc-api-openapi.yml,\n  openapi/evolutionaryscale-forge-folding-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 11\n  by_consequence:\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/generate\n  method: post\n  operationId: generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/batch_generate\n\
  \  method: post\n  operationId: batchGenerate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/encode\n  method: post\n  operationId: encode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/decode\n  method: post\n  operationId: decode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/forward_and_sample\n  method: post\n  operationId: forwardAndSample\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/logits\n  method: post\n  operationId: logits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/esmc/encode\n  method: post\n  operationId: esmcEncode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /api/v1/esmc/logits\n  method: post\n  operationId: esmcLogits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fold\n  method: post\n  operationId: fold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/inverse_fold\n  method: post\n  operationId: inverseFold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/msa\n  method: post\n  operationId: msa\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/agentic-access/evolutionaryscale-agentic-access.yml
summary_line: 11 operations · 11 acting
tags:
- AI
- Artificial Intelligence
- Biology
- Bioinformatics
- Computational Biology
- Drug Discovery
- ESM
- ESM3
- ESM Cambrian
- Foundation Models
- Generative Biology
- Life Sciences
- Machine Learning
- Protein Design
- Protein Folding
- Protein Language Models
- Proteins
- Representation Learning
- Structure Prediction
---
