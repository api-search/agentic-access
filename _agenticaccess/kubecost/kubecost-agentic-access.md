---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 15
api_specs:
- filename: kubecost-allocation-openapi.yml
  format: yaml
  label: Kubecost Allocation API
  slug: allocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-allocation-openapi.yml
- filename: kubecost-assets-openapi.yml
  format: yaml
  label: Kubecost Assets API
  slug: assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-assets-openapi.yml
- filename: kubecost-cloud-cost-openapi.yml
  format: yaml
  label: Kubecost Cloud Cost API
  slug: cloud-cost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-cloud-cost-openapi.yml
- filename: kubecost-budget-openapi.yml
  format: yaml
  label: Kubecost Budget API
  slug: budget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-budget-openapi.yml
- filename: kubecost-forecast-openapi.yml
  format: yaml
  label: Kubecost Forecast API
  slug: forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-forecast-openapi.yml
- filename: kubecost-savings-openapi.yml
  format: yaml
  label: Kubecost Savings API
  slug: savings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/openapi/kubecost-savings-openapi.yml
consequence_counts:
  read: 15
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kubecost Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Kubecost exposes 18 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kubecost
provider_slug: kubecost
slug: kubecost-agentic-access
source_filename: kubecost-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kubecost-allocation-openapi.yml, openapi/kubecost-assets-openapi.yml, openapi/kubecost-budget-openapi.yml,\n  openapi/kubecost-cloud-cost-openapi.yml, openapi/kubecost-forecast-openapi.yml, openapi/kubecost-savings-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 15\n    acting: 3\n  by_consequence:\n    read: 15\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /model/allocation\n  method: get\n  operationId: getAllocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/allocation/totals\n  method: get\n\
  \  operationId: getAllocationTotals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/assets\n  method: get\n  operationId: getAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/assets/totals\n  method: get\n  operationId: getAssetsTotals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/budget\n  method: get\n  operationId: listBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/budget\n  method: post\n  operationId: createBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/budget/{id}\n  method: get\n  operationId: getBudget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/budget/{id}\n  method: put\n  operationId: updateBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/budget/{id}\n  method: delete\n  operationId: deleteBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /model/cloudCost\n  method: get\n  operationId: getCloudCost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/cloudCost/view\n  method: get\n  operationId: getCloudCostView\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/cloudCost/top\n  method: get\n  operationId: getCloudCostTop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/forecast/allocation\n  method: get\n  operationId: getForecastAllocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/savings/clusterSizingETL\n\
  \  method: get\n  operationId: getClusterRightSizing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/savings/requestSizingV2\n  method: get\n  operationId: getContainerRequestRightSizing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/savings/abandonedWorkloads\n  method: get\n  operationId: getAbandonedWorkloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/savings/orphanedDisks\n  method: get\n  operationId: getOrphanedDisks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /model/savings/orphanedIPs\n  method: get\n  operationId: getOrphanedIPs\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubecost/refs/heads/main/agentic-access/kubecost-agentic-access.yml
summary_line: 18 operations · 3 acting
tags:
- Cloud Cost
- Cost Monitoring
- Kubernetes
- Optimization
- Spending
---
