---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 14
api_specs:
- filename: crossplane-kubernetes-api-openapi.yml
  format: yaml
  label: Crossplane Kubernetes API
  slug: crossplane-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossplane/refs/heads/main/openapi/crossplane-kubernetes-api-openapi.yml
consequence_counts:
  physical: 2
  read: 14
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crossplane Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /apis/pkg.crossplane.io/v1beta1/deploymentruntimeconfigs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /apis/pkg.crossplane.io/v1beta1/deploymentruntimeconfigs/{name}
operation_count: 31
overview: 'Crossplane exposes 31 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 15 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crossplane
provider_slug: crossplane
slug: crossplane-agentic-access
source_filename: crossplane-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/crossplane-kubernetes-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 14\n    acting: 17\n  by_consequence:\n    read: 14\n    write: 15\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /apis/apiextensions.crossplane.io/v1/compositions\n  method: get\n  operationId: listCompositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apiextensions.crossplane.io/v1/compositions\n  method: post\n  operationId: createComposition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apiextensions.crossplane.io/v1/compositions/{name}\n  method: get\n  operationId: getComposition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apiextensions.crossplane.io/v1/compositions/{name}\n  method: put\n  operationId: replaceComposition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apiextensions.crossplane.io/v1/compositions/{name}\n  method: delete\n  operationId: deleteComposition\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apiextensions.crossplane.io/v1/compositeresourcedefinitions\n  method: get\n  operationId: listCompositeResourceDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apiextensions.crossplane.io/v1/compositeresourcedefinitions\n  method: post\n  operationId: createCompositeResourceDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apiextensions.crossplane.io/v1/compositeresourcedefinitions/{name}\n\
  \  method: get\n  operationId: getCompositeResourceDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apiextensions.crossplane.io/v1/compositeresourcedefinitions/{name}\n  method: put\n  operationId: replaceCompositeResourceDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apiextensions.crossplane.io/v1/compositeresourcedefinitions/{name}\n  method: delete\n  operationId: deleteCompositeResourceDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apiextensions.crossplane.io/v1/environmentconfigs\n  method: get\n  operationId: listEnvironmentConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apiextensions.crossplane.io/v1/environmentconfigs\n  method: post\n  operationId: createEnvironmentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apiextensions.crossplane.io/v1/environmentconfigs/{name}\n  method: get\n  operationId: getEnvironmentConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /apis/apiextensions.crossplane.io/v1/environmentconfigs/{name}\n  method: delete\n  operationId: deleteEnvironmentConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/pkg.crossplane.io/v1/providers\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/pkg.crossplane.io/v1/providers\n  method: post\n  operationId: createProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /apis/pkg.crossplane.io/v1/providers/{name}\n  method: get\n  operationId: getProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/pkg.crossplane.io/v1/providers/{name}\n  method: put\n  operationId: replaceProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/pkg.crossplane.io/v1/providers/{name}\n  method: delete\n  operationId: deleteProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /apis/pkg.crossplane.io/v1/functions\n  method: get\n  operationId: listFunctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/pkg.crossplane.io/v1/functions\n  method: post\n  operationId: createFunction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/pkg.crossplane.io/v1/functions/{name}\n  method: get\n  operationId: getFunction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/pkg.crossplane.io/v1/functions/{name}\n  method: delete\n  operationId: deleteFunction\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/pkg.crossplane.io/v1/configurations\n  method: get\n  operationId: listConfigurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/pkg.crossplane.io/v1/configurations\n  method: post\n  operationId: createConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/pkg.crossplane.io/v1/configurations/{name}\n  method: get\n  operationId: getConfiguration\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/pkg.crossplane.io/v1/configurations/{name}\n  method: delete\n  operationId: deleteConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/pkg.crossplane.io/v1beta1/deploymentruntimeconfigs\n  method: get\n  operationId: listDeploymentRuntimeConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/pkg.crossplane.io/v1beta1/deploymentruntimeconfigs\n  method: post\n  operationId: createDeploymentRuntimeConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/pkg.crossplane.io/v1beta1/deploymentruntimeconfigs/{name}\n  method: get\n  operationId: getDeploymentRuntimeConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/pkg.crossplane.io/v1beta1/deploymentruntimeconfigs/{name}\n  method: delete\n  operationId: deleteDeploymentRuntimeConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossplane/refs/heads/main/agentic-access/crossplane-agentic-access.yml
summary_line: 31 operations · 17 acting
tags:
- Apache 2.0
- CNCF
- Cloud Native
- Composition
- Control Plane
- Custom Resource Definitions
- Graduated
- Infrastructure as Code
- Kubernetes
- Multi-Cloud
- Open Source
- Platform Engineering
- Providers
---
