---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 16
api_specs:
- filename: chef-channels-api-openapi.yml
  format: yaml
  label: Chef Channels API
  slug: chef-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-channels-api-openapi.yml
- filename: chef-clients-api-openapi.yml
  format: yaml
  label: Chef Clients API
  slug: chef-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-clients-api-openapi.yml
- filename: chef-cookbooks-api-openapi.yml
  format: yaml
  label: Chef Cookbooks API
  slug: chef-cookbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-cookbooks-api-openapi.yml
- filename: chef-data-bags-api-openapi.yml
  format: yaml
  label: Chef Data Bags API
  slug: chef-data-bags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-data-bags-api-openapi.yml
- filename: chef-environments-api-openapi.yml
  format: yaml
  label: Chef Environments API
  slug: chef-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-environments-api-openapi.yml
- filename: chef-iam-api-openapi.yml
  format: yaml
  label: Chef IAM API
  slug: chef-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-iam-api-openapi.yml
- filename: chef-nodes-api-openapi.yml
  format: yaml
  label: Chef Nodes API
  slug: chef-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-nodes-api-openapi.yml
- filename: chef-packages-api-openapi.yml
  format: yaml
  label: Chef Packages API
  slug: chef-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-packages-api-openapi.yml
- filename: chef-profiles-api-openapi.yml
  format: yaml
  label: Chef Profiles API
  slug: chef-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-profiles-api-openapi.yml
- filename: chef-reports-api-openapi.yml
  format: yaml
  label: Chef Reports API
  slug: chef-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-reports-api-openapi.yml
- filename: chef-roles-api-openapi.yml
  format: yaml
  label: Chef Roles API
  slug: chef-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-roles-api-openapi.yml
- filename: chef-scans-api-openapi.yml
  format: yaml
  label: Chef Scans API
  slug: chef-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-scans-api-openapi.yml
- filename: chef-users-api-openapi.yml
  format: yaml
  label: Chef Users API
  slug: chef-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-users-api-openapi.yml
consequence_counts:
  read: 16
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chef Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Chef exposes 22 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chef
provider_slug: chef
slug: chef-agentic-access
source_filename: chef-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chef-automate-api-openapi.yml, openapi/chef-habitat-builder-api-openapi.yml,\n  openapi/chef-infra-server-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 16\n    acting: 6\n  by_consequence:\n    read: 16\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /compliance/profiles\n  method: get\n  operationId: listComplianceProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compliance/scanner/jobs\n  method: post\n  operationId: createScanJob\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compliance/reporting/reports\n  method: post\n  operationId: searchReports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cfgmgmt/nodes\n  method: get\n  operationId: listManagedNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/iam/v2/users\n  method: get\n  operationId: listIamUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /depot/origins/{origin}/pkgs\n  method: get\n  operationId: listOriginPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /depot/pkgs/{origin}/{pkg}\n  method: get\n  operationId: getPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /depot/channels/{origin}\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nodes\n  method: get\n  operationId: listNodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nodes\n  method: post\n  operationId: createNode\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nodes/{nodeName}\n  method: get\n  operationId: getNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nodes/{nodeName}\n  method: put\n  operationId: updateNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nodes/{nodeName}\n  method: delete\n  operationId: deleteNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cookbooks\n  method: get\n  operationId: listCookbooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cookbooks/{cookbookName}\n  method: get\n  operationId: getCookbook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles\n  method: get\n  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles\n  method: post\n  operationId: createRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles/{roleName}\n  method: get\n  operationId: getRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments\n  method: get\n  operationId: listEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data\n  method: get\n  operationId: listDataBags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients\n  method: get\n  operationId: listClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId:\
  \ listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/agentic-access/chef-agentic-access.yml
summary_line: 22 operations · 6 acting
tags:
- Application Delivery
- Automation
- Compliance
- Configuration Management
- DevOps
- DevSecOps
- Habitat
- Infrastructure as Code
- InSpec
---
