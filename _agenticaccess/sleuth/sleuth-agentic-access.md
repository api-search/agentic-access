---
acting_count: 4
action_class_counts:
  acting: 4
api_specs:
- filename: sleuth-openapi.yml
  format: yaml
  label: Sleuth Deployments Registration API
  slug: deployments-registration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/openapi/sleuth-openapi.yml
- filename: sleuth-openapi.yml
  format: yaml
  label: Sleuth Manual Change API
  slug: manual-change-registration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/openapi/sleuth-openapi.yml
- filename: sleuth-openapi.yml
  format: yaml
  label: Sleuth Metric and Incident Impact API
  slug: metric-impact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/openapi/sleuth-openapi.yml
consequence_counts:
  physical: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sleuth Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/{org_slug}/{deployment_slug}/register_deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/{org_slug}/{project_slug}/register_manual_deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/{org_slug}/{project_slug}/{environment_slug}/{impact_source_slug}/register_impact/{api_key}
operation_count: 4
overview: 'Sleuth exposes 4 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sleuth
provider_slug: sleuth
slug: sleuth-agentic-access
source_filename: sleuth-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sleuth-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 4\n  by_consequence:\n    physical: 3\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /deployments/{org_slug}/{deployment_slug}/register_deploy\n  method: post\n  operationId: registerDeploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{org_slug}/{project_slug}/register_manual_deploy\n\
  \  method: post\n  operationId: registerManualChange\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /impact/{impact_id}/register_impact\n  method: post\n  operationId: registerMetricImpact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/{org_slug}/{project_slug}/{environment_slug}/{impact_source_slug}/register_impact/{api_key}\n  method: post\n  operationId: registerIncidentImpact\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/agentic-access/sleuth-agentic-access.yml
summary_line: 4 operations · 4 acting
tags:
- DORA
- DevOps
- Deployment Tracking
- Engineering Metrics
- Continuous Delivery
---
