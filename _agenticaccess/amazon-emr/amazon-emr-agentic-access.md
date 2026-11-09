---
acting_count: 1
action_class_counts:
  acting: 1
api_specs:
- filename: amazon-emr-clusters-api-openapi.yml
  format: yaml
  label: Amazon EMR Clusters API
  slug: amazon-emr-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-clusters-api-openapi.yml
- filename: amazon-emr-auto-termination-policy-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Auto Termination Policy API
  slug: amazon-emr-auto-termination-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-auto-termination-policy-api-openapi.yml
- filename: amazon-emr-instance-fleet-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Instance Fleet API
  slug: amazon-emr-instance-fleet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-instance-fleet-api-openapi.yml
- filename: amazon-emr-instance-group-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Instance Group API
  slug: amazon-emr-instance-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-instance-group-api-openapi.yml
- filename: amazon-emr-managed-scaling-policy-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Managed Scaling Policy API
  slug: amazon-emr-managed-scaling-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-managed-scaling-policy-api-openapi.yml
- filename: amazon-emr-notebook-execution-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Notebook Execution API
  slug: amazon-emr-notebook-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-notebook-execution-api-openapi.yml
- filename: amazon-emr-operations-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Operations API
  slug: amazon-emr-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-operations-api-openapi.yml
- filename: amazon-emr-security-configuration-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Security Configuration API
  slug: amazon-emr-security-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-security-configuration-api-openapi.yml
- filename: amazon-emr-session-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Session API
  slug: amazon-emr-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-session-api-openapi.yml
- filename: amazon-emr-step-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Step API
  slug: amazon-emr-step-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-step-api-openapi.yml
- filename: amazon-emr-studio-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Studio API
  slug: amazon-emr-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-studio-api-openapi.yml
- filename: amazon-emr-studio-session-mapping-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Studio Session Mapping API
  slug: amazon-emr-studio-session-mapping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-studio-session-mapping-api-openapi.yml
consequence_counts:
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Emr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 1
overview: 'Amazon EMR exposes 1 API operation that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon EMR
provider_slug: amazon-emr
slug: amazon-emr-agentic-access
source_filename: amazon-emr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-emr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1\n  by_action_class:\n    acting: 1\n  by_consequence:\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: RunJobFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/amazon-emr/agentic-access/amazon-emr-agentic-access.yml
summary_line: 1 operation · 1 acting
tags:
- Amazon Web Services
- Analytics
- Apache Spark
- Big Data
- Data Processing
- Hadoop
---
