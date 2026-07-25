---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 15
api_specs:
- filename: replicate-accounts-api-openapi.yml
  format: yaml
  label: Replicate Accounts API
  slug: replicate-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-accounts-api-openapi.yml
- filename: replicate-cancel-api-openapi.yml
  format: yaml
  label: Replicate Cancel API
  slug: replicate-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-cancel-api-openapi.yml
- filename: replicate-collections-api-openapi.yml
  format: yaml
  label: Replicate Collections API
  slug: replicate-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-collections-api-openapi.yml
- filename: replicate-deployments-api-openapi.yml
  format: yaml
  label: Replicate Deployments API
  slug: replicate-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-deployments-api-openapi.yml
- filename: replicate-hardware-api-openapi.yml
  format: yaml
  label: Replicate Hardware API
  slug: replicate-hardware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-hardware-api-openapi.yml
- filename: replicate-model-api-openapi.yml
  format: yaml
  label: Replicate Model API
  slug: replicate-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-model-api-openapi.yml
- filename: replicate-models-api-openapi.yml
  format: yaml
  label: Replicate Models API
  slug: replicate-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-models-api-openapi.yml
- filename: replicate-name-api-openapi.yml
  format: yaml
  label: Replicate Name API
  slug: replicate-name-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-name-api-openapi.yml
- filename: replicate-owner-api-openapi.yml
  format: yaml
  label: Replicate Owner API
  slug: replicate-owner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-owner-api-openapi.yml
- filename: replicate-predictions-api-openapi.yml
  format: yaml
  label: Replicate Predictions API
  slug: replicate-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-predictions-api-openapi.yml
- filename: replicate-secrets-api-openapi.yml
  format: yaml
  label: Replicate Secrets API
  slug: replicate-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-secrets-api-openapi.yml
- filename: replicate-slug-api-openapi.yml
  format: yaml
  label: Replicate Slug API
  slug: replicate-slug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-slug-api-openapi.yml
- filename: replicate-training-api-openapi.yml
  format: yaml
  label: Replicate Training API
  slug: replicate-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-training-api-openapi.yml
- filename: replicate-trainings-api-openapi.yml
  format: yaml
  label: Replicate Trainings API
  slug: replicate-trainings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-trainings-api-openapi.yml
- filename: replicate-version-api-openapi.yml
  format: yaml
  label: Replicate Version API
  slug: replicate-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-version-api-openapi.yml
- filename: replicate-webhooks-api-openapi.yml
  format: yaml
  label: Replicate Webhooks API
  slug: replicate-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/openapi/replicate-webhooks-api-openapi.yml
consequence_counts:
  physical: 4
  read: 15
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Replicate Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /deployments/{deployment_owner}/{deployment_name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /deployments/{deployment_owner}/{deployment_name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/{deployment_owner}/{deployment_name}/predictions
operation_count: 27
overview: 'Replicate exposes 27 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 8 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Replicate
provider_slug: replicate
slug: replicate-agentic-access
source_filename: replicate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/replicate-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 15\n    acting: 12\n  by_consequence:\n    read: 15\n    physical: 4\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /account\n  method: get\n  operationId: account.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: collections.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_slug}\n\
  \  method: get\n  operationId: collections.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments\n  method: get\n  operationId: deployments.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments\n  method: post\n  operationId: deployments.create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{deployment_owner}/{deployment_name}\n  method: delete\n  operationId: deployments.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{deployment_owner}/{deployment_name}\n  method: get\n  operationId: deployments.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployments/{deployment_owner}/{deployment_name}\n  method: patch\n  operationId: deployments.update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{deployment_owner}/{deployment_name}/predictions\n\
  \  method: post\n  operationId: deployments.predictions.create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hardware\n  method: get\n  operationId: hardware.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n  method: get\n  operationId: models.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n  method: post\n  operationId: models.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{model_owner}/{model_name}\n  method: delete\n  operationId: models.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{model_owner}/{model_name}\n  method: get\n  operationId: models.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model_owner}/{model_name}/predictions\n  method: post\n  operationId: models.predictions.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{model_owner}/{model_name}/versions\n  method: get\n  operationId: models.versions.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model_owner}/{model_name}/versions/{version_id}\n  method: delete\n  operationId: models.versions.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{model_owner}/{model_name}/versions/{version_id}\n  method: get\n  operationId: models.versions.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model_owner}/{model_name}/versions/{version_id}/trainings\n  method: post\n  operationId: trainings.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /predictions\n  method: get\n  operationId: predictions.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /predictions\n  method: post\n  operationId: predictions.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /predictions/{prediction_id}\n  method: get\n  operationId: predictions.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /predictions/{prediction_id}/cancel\n  method: post\n  operationId: predictions.cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trainings\n  method: get\n  operationId: trainings.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trainings/{training_id}\n  method: get\n  operationId: trainings.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trainings/{training_id}/cancel\n  method: post\n  operationId: trainings.cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/default/secret\n  method: get\n  operationId: webhooks.default.secret.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/agentic-access/replicate-agentic-access.yml
summary_line: 27 operations · 12 acting
tags:
- Artificial Intelligence
- Machine Learning
- Image Generation
- Language Models
- Model Deployment
---
