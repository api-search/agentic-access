---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: amazon-license-manager-license-configurations-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Configurations API
  slug: amazon-license-manager-license-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-configurations-api-openapi.yml
- filename: amazon-license-manager-grant-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager Grant API
  slug: amazon-license-manager-grant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-grant-api-openapi.yml
- filename: amazon-license-manager-license-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager License API
  slug: amazon-license-manager-license-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-api-openapi.yml
- filename: amazon-license-manager-license-asset-group-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager License Asset Group API
  slug: amazon-license-manager-license-asset-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-asset-group-api-openapi.yml
- filename: amazon-license-manager-license-asset-ruleset-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager License Asset Ruleset API
  slug: amazon-license-manager-license-asset-ruleset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-asset-ruleset-api-openapi.yml
- filename: amazon-license-manager-license-conversion-task-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager License Conversion Task API
  slug: amazon-license-manager-license-conversion-task-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-conversion-task-api-openapi.yml
- filename: amazon-license-manager-license-manager-report-generator-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager License Manager Report Generator API
  slug: amazon-license-manager-license-manager-report-generator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-license-manager-report-generator-api-openapi.yml
- filename: amazon-license-manager-operations-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager Operations API
  slug: amazon-license-manager-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-operations-api-openapi.yml
- filename: amazon-license-manager-token-api-openapi.yml
  format: yaml
  label: Amazon License Manager License Manager Token API
  slug: amazon-license-manager-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-license-manager/openapi/amazon-license-manager-token-api-openapi.yml
consequence_counts:
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon License Manager Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Amazon License Manager exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon License Manager
provider_slug: amazon-license-manager
slug: amazon-license-manager-agentic-access
source_filename: amazon-license-manager-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-license-manager-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    write: 3\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /license-configurations\n  method: post\n  operationId: CreateLicenseConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /license-configurations\n  method: get\n  operationId: ListLicenseConfigurations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /license-configurations/{LicenseConfigurationArn}\n  method: get\n  operationId: GetLicenseConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /license-configurations/{LicenseConfigurationArn}\n  method: put\n  operationId: UpdateLicenseConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /license-configurations/{LicenseConfigurationArn}\n  method: delete\n  operationId: DeleteLicenseConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/amazon-license-manager/agentic-access/amazon-license-manager-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Amazon Web Services
- Compliance
- Cost Management
- License Management
- Software Licensing
---
