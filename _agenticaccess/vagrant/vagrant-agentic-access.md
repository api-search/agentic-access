---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 13
api_specs:
- filename: vagrant-cloud-api-openapi.yml
  format: yaml
  label: Vagrant Cloud API
  slug: vagrant-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagrant/refs/heads/main/openapi/vagrant-cloud-api-openapi.yml
- filename: vagrant-hcp-vagrant-box-registry-openapi.yml
  format: yaml
  label: HCP Vagrant Box Registry API
  slug: vagrant-hcp-box-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagrant/refs/heads/main/openapi/vagrant-hcp-vagrant-box-registry-openapi.yml
consequence_counts:
  read: 13
  safety-critical: 1
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Vagrant Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /box/{username}/{name}/version/{version}/revoke
operation_count: 33
overview: 'Vagrant exposes 33 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 19 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vagrant
provider_slug: vagrant
slug: vagrant-agentic-access
source_filename: vagrant-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vagrant-cloud-api-openapi.yml, openapi/vagrant-hcp-vagrant-box-registry-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 13\n    acting: 20\n  by_consequence:\n    read: 13\n    write: 19\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /search\n  method: get\n  operationId: searchBoxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /boxes\n  method: post\n  operationId: createBox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /box/{username}/{name}\n  method: get\n  operationId: readBox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /box/{username}/{name}\n  method: put\n  operationId: updateBox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /box/{username}/{name}\n  method: delete\n  operationId: deleteBox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /box/{username}/{name}/versions\n  method: post\n  operationId: createVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /box/{username}/{name}/version/{version}\n  method: get\n  operationId: readVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /box/{username}/{name}/version/{version}\n  method: put\n  operationId: updateVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /box/{username}/{name}/version/{version}\n  method: delete\n  operationId: deleteVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /box/{username}/{name}/version/{version}/release\n  method: put\n  operationId: releaseVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /box/{username}/{name}/version/{version}/revoke\n  method: put\n  operationId: revokeVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /box/{username}/{name}/version/{version}/providers\n  method: post\n  operationId: createProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /box/{username}/{name}/version/{version}/provider/{provider}\n  method: get\n  operationId: readProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /box/{username}/{name}/version/{version}/provider/{provider}\n  method: put\n  operationId: updateProvider\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /box/{username}/{name}/version/{version}/provider/{provider}\n  method: delete\n  operationId: deleteProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /box/{username}/{name}/version/{version}/provider/{provider}/upload\n  method: get\n  operationId: getUploadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /box/{username}/{name}/version/{version}/provider/{provider}/upload/direct\n\
  \  method: get\n  operationId: getDirectUploadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vagrant/2023-01-01/registry\n  method: post\n  operationId: createRegistry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vagrant/2023-01-01/registry/{registry}\n  method: get\n  operationId: readRegistry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vagrant/2023-01-01/registry/{registry}\n  method: delete\n  operationId: deleteRegistry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vagrant/2023-01-01/registry/{registry}/boxes\n  method: get\n  operationId: listBoxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vagrant/2023-01-01/registry/{registry}/boxes\n  method: post\n  operationId: createBox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vagrant/2023-01-01/registry/{registry}/box/{box}\n  method: get\n  operationId: readBox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /vagrant/2023-01-01/registry/{registry}/box/{box}\n  method: put\n  operationId: updateBox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vagrant/2023-01-01/registry/{registry}/box/{box}\n  method: delete\n  operationId: deleteBox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vagrant/2023-01-01/registry/{registry}/box/{box}/versions\n  method: get\n  operationId: listVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /vagrant/2023-01-01/registry/{registry}/box/{box}/versions\n  method: post\n  operationId: createVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vagrant/2023-01-01/registry/{registry}/box/{box}/version/{version}\n  method: get\n  operationId: readVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vagrant/2023-01-01/registry/{registry}/box/{box}/version/{version}\n  method: delete\n  operationId: deleteVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vagrant/2023-01-01/registry/{registry}/box/{box}/version/{version}/providers\n  method: get\n  operationId: listProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vagrant/2023-01-01/registry/{registry}/box/{box}/version/{version}/providers\n  method: post\n  operationId: createProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vagrant/2023-01-01/registry/{registry}/box/{box}/version/{version}/provider/{provider}\n  method: get\n  operationId: readProvider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vagrant/2023-01-01/registry/{registry}/box/{box}/version/{version}/provider/{provider}\n  method: delete\n  operationId: deleteProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vagrant/refs/heads/main/agentic-access/vagrant-agentic-access.yml
summary_line: 33 operations · 20 acting · 1 human-in-the-loop
tags:
- DevOps
- Virtualization
- Development Environments
- Boxes
- Cloud
- HashiCorp
- Infrastructure
---
