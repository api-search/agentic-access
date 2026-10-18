---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-api-api-openapi.yml
  format: yaml
  label: AWS Elastic Beanstalk Amazon Elastic Beanstalk AWS Elastic Beanstalk API
  slug: aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-elastic-beanstalk/refs/heads/main/openapi/aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-api-api-openapi.yml
- filename: aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-create-api-openapi.yml
  format: yaml
  label: 'AWS Elastic Beanstalk Amazon Elastic Beanstalk AWS Elastic Beanstalk #Create… API'
  slug: aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-elastic-beanstalk/refs/heads/main/openapi/aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-create-api-openapi.yml
- filename: aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-describe-api-openapi.yml
  format: yaml
  label: 'AWS Elastic Beanstalk Amazon Elastic Beanstalk AWS Elastic Beanstalk #Describe… API'
  slug: aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-describe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-elastic-beanstalk/refs/heads/main/openapi/aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-describe-api-openapi.yml
- filename: aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-update-api-openapi.yml
  format: yaml
  label: 'AWS Elastic Beanstalk Amazon Elastic Beanstalk AWS Elastic Beanstalk #Update… API'
  slug: aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-elastic-beanstalk/refs/heads/main/openapi/aws-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-update-api-openapi.yml
consequence_counts:
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aws Elastic Beanstalk Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'AWS Elastic Beanstalk exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AWS Elastic Beanstalk
provider_slug: aws-elastic-beanstalk
slug: aws-elastic-beanstalk-agentic-access
source_filename: aws-elastic-beanstalk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: generated\nsource: openapi/amazon-elastic-beanstalk-amazon-elastic-beanstalk-aws-elastic-beanstalk-api-api-openapi.yml,\n  openapi/amazon-elastic-beanstalk-createenvironment-api-openapi.yml, openapi/amazon-elastic-beanstalk-describeenvironments-api-openapi.yml,\n  openapi/amazon-elastic-beanstalk-updateenvironment-api-openapi.yml, openapi/aws-elastic-beanstalk-aws-elastic-beanstalk-api-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    write: 4\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: describeApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#CreateEnvironment\n  method: post\n  operationId: createEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeEnvironments\n  method: get\n  operationId: describeEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /#UpdateEnvironment\n  method: post\n  operationId: updateEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: invokeAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-elastic-beanstalk/refs/heads/main/agentic-access/aws-elastic-beanstalk-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- Platform-as-a-Service
- Application Deployment
- Auto-Scaling
- Cloud
- DevOps
---
