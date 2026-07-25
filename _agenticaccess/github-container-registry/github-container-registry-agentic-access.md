---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 11
api_specs:
- filename: github-container-registry-organization-packages-api-openapi.yml
  format: yaml
  label: GitHub Container Registry Organization Packages API
  slug: github-container-registry-organization-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-container-registry/refs/heads/main/openapi/github-container-registry-organization-packages-api-openapi.yml
- filename: github-container-registry-user-namespace-packages-api-openapi.yml
  format: yaml
  label: GitHub Container Registry User Namespace Packages API
  slug: github-container-registry-user-namespace-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-container-registry/refs/heads/main/openapi/github-container-registry-user-namespace-packages-api-openapi.yml
- filename: github-container-registry-user-packages-api-openapi.yml
  format: yaml
  label: GitHub Container Registry User Packages API
  slug: github-container-registry-user-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-container-registry/refs/heads/main/openapi/github-container-registry-user-packages-api-openapi.yml
consequence_counts:
  read: 11
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Github Container Registry Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'GitHub Container Registry exposes 18 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GitHub Container Registry
provider_slug: github-container-registry
slug: github-container-registry-agentic-access
source_filename: github-container-registry-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/github-container-registry-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 11\n    acting: 7\n  by_consequence:\n    read: 11\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /orgs/{org}/packages\n  method: get\n  operationId: listOrgPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/packages/{package_type}/{package_name}\n  method: get\n  operationId: getOrgPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /orgs/{org}/packages/{package_type}/{package_name}\n  method: delete\n  operationId: deleteOrgPackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/packages/{package_type}/{package_name}/restore\n  method: post\n  operationId: restoreOrgPackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/packages/{package_type}/{package_name}/versions\n  method: get\n  operationId: listOrgPackageVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/packages/{package_type}/{package_name}/versions/{package_version_id}\n  method: get\n  operationId: getOrgPackageVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/packages/{package_type}/{package_name}/versions/{package_version_id}\n  method: delete\n  operationId: deleteOrgPackageVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org}/packages/{package_type}/{package_name}/versions/{package_version_id}/restore\n  method: post\n  operationId: restoreOrgPackageVersion\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/packages\n  method: get\n  operationId: listUserPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/packages/{package_type}/{package_name}\n  method: get\n  operationId: getUserPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/packages/{package_type}/{package_name}\n  method: delete\n  operationId: deleteUserPackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /user/packages/{package_type}/{package_name}/restore\n  method: post\n  operationId: restoreUserPackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/packages/{package_type}/{package_name}/versions\n  method: get\n  operationId: listUserPackageVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/packages/{package_type}/{package_name}/versions/{package_version_id}\n  method: get\n  operationId: getUserPackageVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /user/packages/{package_type}/{package_name}/versions/{package_version_id}\n  method: delete\n  operationId: deleteUserPackageVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{username}/packages\n  method: get\n  operationId: listPackagesForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{username}/packages/{package_type}/{package_name}\n  method: get\n  operationId: getPackageForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{username}/packages/{package_type}/{package_name}/versions\n  method: get\n \
  \ operationId: listPackageVersionsForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-container-registry/refs/heads/main/agentic-access/github-container-registry-agentic-access.yml
summary_line: 18 operations · 7 acting
tags:
- Container Images
- Containers
- GitHub
- Packages
- Registry
---
