---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 5
api_specs:
- filename: amazon-simspace-weaver-createsnapshot-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Createsnapshot API
  slug: amazon-simspace-weaver-createsnapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-createsnapshot-api-openapi.yml
- filename: amazon-simspace-weaver-deleteapp-app-domain-simulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Deleteapp#app&domain&simulation API
  slug: amazon-simspace-weaver-deleteapp-app-domain-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-deleteapp-app-domain-simulation-api-openapi.yml
- filename: amazon-simspace-weaver-deletesimulation-simulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Deletesimulation#simulation API
  slug: amazon-simspace-weaver-deletesimulation-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-deletesimulation-simulation-api-openapi.yml
- filename: amazon-simspace-weaver-describeapp-app-domain-simulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Describeapp#app&domain&simulation API
  slug: amazon-simspace-weaver-describeapp-app-domain-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-describeapp-app-domain-simulation-api-openapi.yml
- filename: amazon-simspace-weaver-describesimulation-simulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Describesimulation#simulation API
  slug: amazon-simspace-weaver-describesimulation-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-describesimulation-simulation-api-openapi.yml
- filename: amazon-simspace-weaver-listapps-simulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Listapps#simulation API
  slug: amazon-simspace-weaver-listapps-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-listapps-simulation-api-openapi.yml
- filename: amazon-simspace-weaver-listsimulations-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Listsimulations API
  slug: amazon-simspace-weaver-listsimulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-listsimulations-api-openapi.yml
- filename: amazon-simspace-weaver-startapp-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Startapp API
  slug: amazon-simspace-weaver-startapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-startapp-api-openapi.yml
- filename: amazon-simspace-weaver-startclock-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Startclock API
  slug: amazon-simspace-weaver-startclock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-startclock-api-openapi.yml
- filename: amazon-simspace-weaver-startsimulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Startsimulation API
  slug: amazon-simspace-weaver-startsimulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-startsimulation-api-openapi.yml
- filename: amazon-simspace-weaver-stopapp-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Stopapp API
  slug: amazon-simspace-weaver-stopapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-stopapp-api-openapi.yml
- filename: amazon-simspace-weaver-stopclock-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Stopclock API
  slug: amazon-simspace-weaver-stopclock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-stopclock-api-openapi.yml
- filename: amazon-simspace-weaver-stopsimulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Stopsimulation API
  slug: amazon-simspace-weaver-stopsimulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-stopsimulation-api-openapi.yml
- filename: amazon-simspace-weaver-tags-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Tags API
  slug: amazon-simspace-weaver-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-tags-api-openapi.yml
consequence_counts:
  read: 5
  safety-critical: 3
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Simspace Weaver Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /stopapp
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /stopclock
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /stopsimulation
operation_count: 16
overview: 'Amazon SimSpace Weaver exposes 16 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 8 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
slug: amazon-simspace-weaver-agentic-access
source_filename: amazon-simspace-weaver-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-simspace-weaver.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 11\n    connected: 5\n  by_consequence:\n    write: 8\n    read: 5\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /createsnapshot\n  method: post\n  operationId: CreateSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deleteapp#app&domain&simulation\n  method: delete\n  operationId: DeleteApp\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deletesimulation#simulation\n  method: delete\n  operationId: DeleteSimulation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /describeapp#app&domain&simulation\n  method: get\n  operationId: DescribeApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /describesimulation#simulation\n  method: get\n  operationId: DescribeSimulation\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listapps#simulation\n  method: get\n  operationId: ListApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listsimulations\n  method: get\n  operationId: ListSimulations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{ResourceArn}\n  method: get\n  operationId: ListTagsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{ResourceArn}\n  method: post\n  operationId: TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /startapp\n  method: post\n  operationId: StartApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /startclock\n  method: post\n  operationId: StartClock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /startsimulation\n  method: post\n  operationId: StartSimulation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stopapp\n  method: post\n  operationId: StopApp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /stopclock\n  method: post\n  operationId: StopClock\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /stopsimulation\n  method: post\n  operationId: StopSimulation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tags/{ResourceArn}#tagKeys\n  method: delete\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/agentic-access/amazon-simspace-weaver-agentic-access.yml
summary_line: 16 operations · 11 acting · 3 human-in-the-loop
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
---
