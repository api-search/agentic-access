---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 28
api_specs:
- filename: crowddev-cdp-public-openapi.yml
  format: yaml
  label: CDP Public API
  slug: cdp-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-cdp-public-openapi.yml
consequence_counts:
  physical: 10
  read: 28
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Crowddev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /members/{memberId}/project-affiliations/{projectId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /akrites/packages:batch-stewardship
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /akrites/stewardships/open
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /akrites/stewardships/{id}/assign
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /akrites/stewardships/{id}/escalate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /akrites/stewardships/{id}/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /packages:batch-stewardship
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /stewardships/open
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /stewardships/{id}/assign
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /stewardships/{id}/escalate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /stewardships/{id}/status
operation_count: 56
overview: 'Crowd.dev exposes 56 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 17 write, 10 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crowd.dev
provider_slug: crowddev
slug: crowddev-agentic-access
source_filename: crowddev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/crowddev-cdp-akrites-external-openapi.yml, openapi/crowddev-cdp-akrites-openapi.yml,\n  openapi/crowddev-cdp-ossprey-openapi.yml, openapi/crowddev-cdp-packages-openapi.yml, openapi/crowddev-cdp-public-openapi.yml,\n  openapi/crowddev-cdp-stewardships-openapi.yml, openapi/crowddev-cm-id-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 56\n  by_action_class:\n    connected: 28\n    acting: 28\n  by_consequence:\n    read: 28\n    write: 17\n    physical: 10\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /akrites-external/packages/detail\n  method: get\n  operationId: getPackageDetail\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - read:packages\n    - read:stewardships\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites-external/packages/detail:batch\n  method: post\n  operationId: getPackageDetailBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:packages\n    - read:stewardships\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /akrites-external/advisories/detail\n  method: get\n  operationId: getAdvisoryDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:packages\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites-external/advisories/detail:batch\n  method: post\n  operationId: getAdvisoryDetailBatch\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - read:packages\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /akrites-external/contacts/detail\n  method: get\n  operationId: getContactDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:maintainer-roles\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites-external/contacts/detail:batch\n  method: post\n  operationId: getContactDetailBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:maintainer-roles\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /akrites/metrics\n  method: get\n\
  \  operationId: getAkritesMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites/activity\n  method: get\n  operationId: getAkritesActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites/packages\n  method: get\n  operationId: listAkritesPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites/packages/scatter\n  method: get\n  operationId: getAkritesPackagesScatter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites/packages/metrics\n  method: get\n  operationId: getAkritesPackagesMetrics\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites/packages/detail\n  method: get\n  operationId: getAkritesPackageDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites/packages/advisories\n  method: get\n  operationId: getAkritesPackageAdvisories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites/packages/history\n  method: get\n  operationId: getAkritesPackageHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites/packages:batch-stewardship\n  method: post\n  operationId: batchGetStewardship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /akrites/stewardships/me/packages\n  method: get\n  operationId: getMyPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites/stewardships/me/activity\n  method: get\n  operationId: getMyActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /akrites/stewardships/open\n  method: post\n  operationId: openStewardship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /akrites/stewardships/{id}/assign\n  method: post\n  operationId: assignSteward\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /akrites/stewardships/{id}/escalate\n  method: post\n  operationId: escalateStewardship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /akrites/stewardships/{id}/status\n\
  \  method: patch\n  operationId: updateStewardshipStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ossprey/metrics\n  method: get\n  operationId: getOsspreyMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ossprey/activity\n  method: get\n  operationId: listStewardshipActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ossprey/packages\n  method: get\n  operationId: listOsspreyPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ossprey/packages/scatter\n  method: get\n  operationId: getOsspreyPackagesScatter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages\n  method: get\n  operationId: listPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:packages\n    - read:stewardships\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/metrics\n  method: get\n  operationId: getPackagesMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:packages\n    - read:stewardships\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/detail\n  method: get\n  operationId: getPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - read:packages\n    - read:stewardships\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages:batch-stewardship\n  method: post\n  operationId: batchGetStewardship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - read:stewardships\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members\n  method: post\n  operationId: createMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:members\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/resolve\n  method: post\n  operationId:\
  \ resolveMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:members\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/{memberId}/identities\n  method: get\n  operationId: getMemberIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:member-identities\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members/{memberId}/identities\n  method: post\n  operationId: createMemberIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:member-identities\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /members/{memberId}/identities/{identityId}\n  method: patch\n  operationId: verifyMemberIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:member-identities\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/{memberId}/maintainer-roles\n  method: get\n  operationId: getMemberMaintainerRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:maintainer-roles\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members/{memberId}/work-experiences\n  method: get\n  operationId: getMemberWorkExperiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:work-experiences\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /members/{memberId}/work-experiences\n  method: post\n  operationId: createMemberWorkExperience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:work-experiences\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/{memberId}/work-experiences/{workExperienceId}\n  method: put\n  operationId: updateMemberWorkExperience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:work-experiences\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/{memberId}/work-experiences/{workExperienceId}\n  method: patch\n  operationId: verifyMemberWorkExperience\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:work-experiences\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/{memberId}/work-experiences/{workExperienceId}\n  method: delete\n  operationId: deleteMemberWorkExperience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:work-experiences\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/{memberId}/project-affiliations\n  method: get\n  operationId: getMemberProjectAffiliations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:project-affiliations\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /members/{memberId}/project-affiliations/{projectId}\n  method: patch\n  operationId: patchMemberProjectAffiliation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - write:project-affiliations\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /organizations\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:organizations\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: post\n  operationId: createOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:organizations\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /affiliations\n  method: post\n  operationId: getBulkAffiliations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /affiliations/{githubHandle}\n  method: get\n  operationId: getAffiliationByHandle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stewardships/open\n  method: post\n  operationId: openStewardship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write:stewardships\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stewardships/{id}/assign\n  method: post\n  operationId: assignSteward\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write:stewardships\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stewardships/{id}/escalate\n  method: post\n  operationId: escalateStewardship\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write:stewardships\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stewardships/{id}/status\n  method: patch\n  operationId: updateStewardshipStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write:stewardships\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /member/{memberId}/organization\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /member/{memberId}/organization\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /member/{memberId}/organization/{workHistoryId}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /member/{memberId}/organization/{workHistoryId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /member/{memberId}/affiliation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /member/{memberId}/affiliation\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/agentic-access/crowddev-agentic-access.yml
summary_line: 56 operations · 28 acting · 1 human-in-the-loop
tags:
- Company
- Community
- Developer Relations
- Developer Data Platform
- Identity Resolution
- Open Source
- Community Data Platform
- Open Source Intelligence
---
