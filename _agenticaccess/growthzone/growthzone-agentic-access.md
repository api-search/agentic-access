---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 17
api_specs:
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Contacts API
  slug: growthzone-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Memberships API
  slug: growthzone-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Groups & Directory API
  slug: growthzone-groups-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Scheduled Billing API
  slug: growthzone-scheduled-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Certifications API
  slug: growthzone-certifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone Events API
  slug: growthzone-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
- filename: growthzone-openapi.yml
  format: yaml
  label: GrowthZone OAuth / OpenID Connect (SSO) API
  slug: growthzone-oauth-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/openapi/growthzone-openapi.yml
consequence_counts:
  physical: 6
  read: 17
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Growthzone Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /memberships/all
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /scheduledbilling/membershiptype/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /scheduledbilling/membershiptype/items/export
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /scheduledbilling/membershiptype/items/run
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /scheduledbilling/membershiptype/items/run/setup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /scheduledbilling/membershiptype/run/history/download/{systemjobid}
operation_count: 25
overview: 'GrowthZone exposes 25 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 2 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GrowthZone
provider_slug: growthzone
slug: growthzone-agentic-access
source_filename: growthzone-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/growthzone-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 17\n    acting: 8\n  by_consequence:\n    read: 17\n    physical: 6\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/delta\n  method: get\n  operationId: listChangedContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/person/{contactId}\n\
  \  method: get\n  operationId: getPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/PersonSummary/{contactId}\n  method: get\n  operationId: getPersonSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/OrgGeneral/{contactId}\n  method: get\n  operationId: getOrganizationGeneral\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/ContactAddresses/{contactId}\n  method: get\n  operationId: getContactAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/PrimaryContact/Emails/{primaryContactId}\n  method: get\n  operationId:\
  \ getPrimaryContactEmails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/lookup/{contactId}/contactwebsites\n  method: get\n  operationId: getContactWebsites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contactId}/NotesAndFields\n  method: get\n  operationId: getContactNotesAndFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/person/{contactId}/categorySummary\n  method: get\n  operationId: getPersonCategorySummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/person/{contactId}/memberships\n  method: get\n  operationId:\
  \ getPersonMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/org/{contactId}/groups\n  method: get\n  operationId: getOrganizationGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memberships/types\n  method: get\n  operationId: listMembershipTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memberships/all\n  method: post\n  operationId: listAllMemberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /GroupsApi_GetGroupsByCategories\n  method: post\n  operationId: getGroupsByCategories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{groupId}/members\n  method: get\n  operationId: listGroupMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /certifications/{certificationContactId}/Components/{certificationComponentId}/Completed\n  method: post\n  operationId: markCertificationComponentCompleted\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduledbilling/membershiptype/items\n  method: post\n  operationId: previewScheduledBillingItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduledbilling/membershiptype/items/export\n  method: post\n  operationId: exportScheduledBillingItems\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduledbilling/membershiptype/items/run/setup\n\
  \  method: post\n  operationId: setupScheduledBillingRun\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduledbilling/membershiptype/items/run\n  method: post\n  operationId: runScheduledBilling\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduledbilling/membershiptype/run/history\n  method: get\n  operationId: listScheduledBillingRunHistory\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduledbilling/membershiptype/run/history/download/{systemjobid}\n  method: post\n  operationId: downloadScheduledBillingRun\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growthzone/refs/heads/main/agentic-access/growthzone-agentic-access.yml
summary_line: 25 operations · 8 acting
tags:
- Association Management
- AMS
- Membership Management
- Chambers of Commerce
- ChamberMaster
- Member Directory
- Events
- Billing
---
