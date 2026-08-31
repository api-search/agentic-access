---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 22
api_specs:
- filename: openstack-domains-api-openapi.yml
  format: yaml
  label: OpenStack Domains API
  slug: openstack-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-domains-api-openapi.yml
- filename: openstack-endpoints-api-openapi.yml
  format: yaml
  label: OpenStack Endpoints API
  slug: openstack-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-endpoints-api-openapi.yml
- filename: openstack-flavors-api-openapi.yml
  format: yaml
  label: OpenStack Flavors API
  slug: openstack-flavors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-flavors-api-openapi.yml
- filename: openstack-groups-api-openapi.yml
  format: yaml
  label: OpenStack Groups API
  slug: openstack-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-groups-api-openapi.yml
- filename: openstack-images-api-openapi.yml
  format: yaml
  label: OpenStack Images API
  slug: openstack-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-images-api-openapi.yml
- filename: openstack-keypairs-api-openapi.yml
  format: yaml
  label: OpenStack Keypairs API
  slug: openstack-keypairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-keypairs-api-openapi.yml
- filename: openstack-projects-api-openapi.yml
  format: yaml
  label: OpenStack Projects API
  slug: openstack-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-projects-api-openapi.yml
- filename: openstack-roles-api-openapi.yml
  format: yaml
  label: OpenStack Roles API
  slug: openstack-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-roles-api-openapi.yml
- filename: openstack-server-actions-api-openapi.yml
  format: yaml
  label: OpenStack Server Actions API
  slug: openstack-server-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-server-actions-api-openapi.yml
- filename: openstack-servers-api-openapi.yml
  format: yaml
  label: OpenStack Servers API
  slug: openstack-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-servers-api-openapi.yml
- filename: openstack-services-api-openapi.yml
  format: yaml
  label: OpenStack Services API
  slug: openstack-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-services-api-openapi.yml
- filename: openstack-tokens-api-openapi.yml
  format: yaml
  label: OpenStack Tokens API
  slug: openstack-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-tokens-api-openapi.yml
- filename: openstack-users-api-openapi.yml
  format: yaml
  label: OpenStack Users API
  slug: openstack-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-users-api-openapi.yml
- filename: openstack-versions-api-openapi.yml
  format: yaml
  label: OpenStack Versions API
  slug: openstack-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-versions-api-openapi.yml
consequence_counts:
  read: 22
  safety-critical: 1
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Openstack Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /auth/tokens
operation_count: 41
overview: 'OpenStack exposes 41 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 18 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenStack
provider_slug: openstack
slug: openstack-agentic-access
source_filename: openstack-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openstack-keystone-openapi.yml, openapi/openstack-nova-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    acting: 19\n    connected: 22\n  by_consequence:\n    write: 18\n    read: 22\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /auth/tokens\n  method: post\n  operationId: issueToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/tokens\n  method: get\n  operationId: validateToken\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/tokens\n  method: head\n  operationId: checkToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/tokens\n  method: delete\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId: createUser\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_id}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: createProject\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}\n  method: patch\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains\n  method: post\n  operationId: createDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles\n  method: get\n  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles\n  method: post\n  operationId:\
  \ createRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /role_assignments\n  method: get\n  operationId: listRoleAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: post\n  operationId: createService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /endpoints\n  method: get\n  operationId: listEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /endpoints\n  method: post\n  operationId: createEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: listVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers\n  method: get\n  operationId: listServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /servers\n  method: post\n  operationId: createServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/detail\n  method: get\n  operationId: listServersDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/{server_id}\n  method: get\n  operationId: getServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /servers/{server_id}\n  method: put\n  operationId: updateServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{server_id}\n  method: delete\n  operationId: deleteServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /servers/{server_id}/action\n  method: post\n  operationId: serverAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flavors\n  method: get\n  operationId: listFlavors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flavors/detail\n  method: get\n  operationId: listFlavorsDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flavors/{flavor_id}\n  method: get\n  operationId: getFlavor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images\n  method: get\n  operationId: listImagesProxy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /os-keypairs\n  method: get\n  operationId: listKeypairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /os-keypairs\n  method: post\n  operationId: createKeypair\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /os-keypairs/{name}\n  method: get\n  operationId: getKeypair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /os-keypairs/{name}\n  method: delete\n  operationId: deleteKeypair\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/agentic-access/openstack-agentic-access.yml
summary_line: 41 operations · 19 acting · 1 human-in-the-loop
tags:
- Cloud Platform
- Infrastructure as a Service
- Open-Source
- Virtualization
- Linux Foundation
---
