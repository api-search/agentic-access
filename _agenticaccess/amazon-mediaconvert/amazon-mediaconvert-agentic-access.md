---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 10
api_specs:
- filename: amazon-mediaconvert-certificates-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Certificates API
  slug: amazon-mediaconvert-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-certificates-api-openapi.yml
- filename: amazon-mediaconvert-endpoints-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Endpoints API
  slug: amazon-mediaconvert-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-endpoints-api-openapi.yml
- filename: amazon-mediaconvert-jobs-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Jobs API
  slug: amazon-mediaconvert-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-jobs-api-openapi.yml
- filename: amazon-mediaconvert-jobtemplates-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert JobTemplates API
  slug: amazon-mediaconvert-jobtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-jobtemplates-api-openapi.yml
- filename: amazon-mediaconvert-policy-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Policy API
  slug: amazon-mediaconvert-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-policy-api-openapi.yml
- filename: amazon-mediaconvert-presets-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Presets API
  slug: amazon-mediaconvert-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-presets-api-openapi.yml
- filename: amazon-mediaconvert-queues-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Queues API
  slug: amazon-mediaconvert-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-queues-api-openapi.yml
- filename: amazon-mediaconvert-tags-api-openapi.yml
  format: yaml
  label: Amazon MediaConvert Tags API
  slug: amazon-mediaconvert-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/openapi/amazon-mediaconvert-tags-api-openapi.yml
consequence_counts:
  read: 10
  safety-critical: 3
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Mediaconvert Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2017-08-29/presets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /2017-08-29/presets/{name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /2017-08-29/presets/{name}
operation_count: 28
overview: 'Amazon MediaConvert exposes 28 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 15 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
slug: amazon-mediaconvert-agentic-access
source_filename: amazon-mediaconvert-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-mediaconvert-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 18\n    connected: 10\n  by_consequence:\n    write: 15\n    read: 10\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /2017-08-29/certificates\n  method: post\n  operationId: AssociateCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/jobs/{id}\n  method: delete\n  operationId:\
  \ CancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/jobs/{id}\n  method: get\n  operationId: GetJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2017-08-29/jobs\n  method: post\n  operationId: CreateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/jobs\n  method: get\n  operationId: ListJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2017-08-29/jobTemplates\n  method: post\n  operationId: CreateJobTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/jobTemplates\n  method: get\n  operationId: ListJobTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2017-08-29/presets\n  method: post\n  operationId: CreatePreset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /2017-08-29/presets\n  method: get\n  operationId: ListPresets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2017-08-29/queues\n  method: post\n  operationId: CreateQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/queues\n  method: get\n  operationId: ListQueues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2017-08-29/jobTemplates/{name}\n  method: delete\n  operationId: DeleteJobTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/jobTemplates/{name}\n  method: get\n  operationId: GetJobTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2017-08-29/jobTemplates/{name}\n  method: put\n  operationId: UpdateJobTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/policy\n  method: delete\n  operationId: DeletePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/policy\n  method: get\n  operationId: GetPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2017-08-29/policy\n  method: put\n  operationId: PutPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/presets/{name}\n  method: delete\n  operationId: DeletePreset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /2017-08-29/presets/{name}\n  method: get\n  operationId: GetPreset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2017-08-29/presets/{name}\n  method: put\n  operationId: UpdatePreset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /2017-08-29/queues/{name}\n  method: delete\n  operationId: DeleteQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/queues/{name}\n  method: get\n  operationId: GetQueue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2017-08-29/queues/{name}\n  method: put\n  operationId: UpdateQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/endpoints\n  method: post\n  operationId: DescribeEndpoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /2017-08-29/certificates/{arn}\n  method: delete\n  operationId: DisassociateCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/tags/{arn}\n  method: get\n  operationId: ListTagsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2017-08-29/tags/{arn}\n  method: put\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2017-08-29/tags\n  method: post\n  operationId:\
  \ TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/agentic-access/amazon-mediaconvert-agentic-access.yml
summary_line: 28 operations · 18 acting · 3 human-in-the-loop
tags:
- Broadcasting
- Media Processing
- Media
---
