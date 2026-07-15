---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: apache-software-foundation-projects-api-openapi.yml
  format: yaml
  label: Apache Software Foundation Projects API
  slug: projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-software-foundation/refs/heads/main/openapi/apache-software-foundation-projects-api-openapi.yml
- filename: apache-software-foundation-whimsy-api-openapi.yml
  format: yaml
  label: Apache Software Foundation Whimsy Public Data API
  slug: whimsy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-software-foundation/refs/heads/main/openapi/apache-software-foundation-whimsy-api-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apache Software Foundation Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Apache Software Foundation exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apache Software Foundation
provider_slug: apache-software-foundation
slug: apache-software-foundation-agentic-access
source_filename: apache-software-foundation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/apache-software-foundation-projects-api-openapi.yml, openapi/apache-software-foundation-whimsy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /foundation/groups.json\n  method: get\n  operationId: getGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foundation/committees.json\n  method: get\n  operationId: getCommittees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /foundation/projects.json\n  method: get\n  operationId: getProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foundation/releases.json\n  method: get\n  operationId: getReleases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foundation/podlings.json\n  method: get\n  operationId: getPodlings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foundation/people.json\n  method: get\n  operationId: getPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /foundation/people_name.json\n  method: get\n  operationId: getPeopleNames\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /committee-info.json\n  method: get\n  operationId: getCommitteeInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_ldap_committees.json\n  method: get\n  operationId: getPublicLdapCommittees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_ldap_groups.json\n  method: get\n  operationId: getPublicLdapGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_ldap_people.json\n  method: get\n  operationId: getPublicLdapPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /icla-info.json\n  method: get\n  operationId: getIclaInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /member-info.json\n  method: get\n  operationId: getMemberInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public_podlings.json\n  method: get\n  operationId: getPublicPodlings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-software-foundation/refs/heads/main/agentic-access/apache-software-foundation-agentic-access.yml
summary_line: 14 operations
tags:
- ASF
- Open Source
- Governance
- Projects
- Apache
---
