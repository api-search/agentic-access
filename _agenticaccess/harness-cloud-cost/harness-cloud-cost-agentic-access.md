---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 10
api_specs:
- filename: harness-cloud-cost-anomalies-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Anomalies API
  slug: harness-cloud-cost-anomalies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-anomalies-api-openapi.yml
- filename: harness-cloud-cost-budgets-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Budgets API
  slug: harness-cloud-cost-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-budgets-api-openapi.yml
- filename: harness-cloud-cost-connectors-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Connectors API
  slug: harness-cloud-cost-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-connectors-api-openapi.yml
- filename: harness-cloud-cost-cost-categories-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Cost Categories API
  slug: harness-cloud-cost-cost-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-cost-categories-api-openapi.yml
- filename: harness-cloud-cost-perspectives-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Perspectives API
  slug: harness-cloud-cost-perspectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-perspectives-api-openapi.yml
- filename: harness-cloud-cost-recommendations-api-openapi.yml
  format: yaml
  label: Harness Cloud Cost Management Recommendations API
  slug: harness-cloud-cost-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/openapi/harness-cloud-cost-recommendations-api-openapi.yml
consequence_counts:
  read: 10
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Harness Cloud Cost Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Harness Cloud Cost Management exposes 17 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Harness Cloud Cost Management
provider_slug: harness-cloud-cost
slug: harness-cloud-cost-agentic-access
source_filename: harness-cloud-cost-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/harness-cloud-cost-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 10\n    acting: 7\n  by_consequence:\n    read: 10\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /ccm/api/perspective\n  method: get\n  operationId: listPerspectives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccm/api/perspective\n  method: post\n  operationId: createPerspective\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ccm/api/perspective/{perspectiveId}\n  method: get\n  operationId: getPerspective\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccm/api/perspective/{perspectiveId}\n  method: put\n  operationId: updatePerspective\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ccm/api/perspective/{perspectiveId}\n  method: delete\n  operationId: deletePerspective\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ccm/api/budgets\n  method: get\n  operationId: listBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccm/api/budgets\n  method: post\n  operationId: createBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ccm/api/budgets/{budgetId}\n  method: get\n  operationId: getBudget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccm/api/budgets/{budgetId}\n  method: put\n  operationId: updateBudget\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ccm/api/budgets/{budgetId}\n  method: delete\n  operationId: deleteBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ccm/api/recommendation/overview/list\n  method: get\n  operationId: listRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccm/api/recommendation/{recommendationId}\n  method: get\n  operationId: getRecommendation\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccm/api/anomaly\n  method: get\n  operationId: listAnomalies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccm/api/anomaly/{anomalyId}\n  method: get\n  operationId: getAnomaly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccm/api/business-mapping\n  method: get\n  operationId: listCostCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccm/api/business-mapping\n  method: post\n  operationId: createCostCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ng/api/connectors\n  method: get\n  operationId: listConnectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harness-cloud-cost/refs/heads/main/agentic-access/harness-cloud-cost-agentic-access.yml
summary_line: 17 operations · 7 acting
tags:
- Anomaly Detection
- Budgets
- Cloud Cost Management
- FinOps
- Kubernetes
- Recommendations
---
