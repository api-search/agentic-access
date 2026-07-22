---
acting_count: 81
action_class_counts:
  acting: 81
  connected: 81
api_specs:
- filename: sedna-openapi.json
  format: json
  label: Sedna API
  slug: sedna-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-openapi.json
consequence_counts:
  physical: 42
  read: 81
  safety-critical: 4
  write: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Sedna Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2019-01-01/team/{id}/relationships/disable-send-users
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /2019-01-01/team/{id}/relationships/disable-send-users
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2019-01-01/user/{id}/relationships/disable-send-teams
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /2019-01-01/user/{id}/relationships/disable-send-teams
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-01-01/category-tag/{id}/relationships/message
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /2019-01-01/category-tag/{id}/relationships/message
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-01-01/category-tag/{id}/relationships/team
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /2019-01-01/category-tag/{id}/relationships/team
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /2019-01-01/category-tag/{id}/relationships/team
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-01-01/contact-group/{id}/relationships/contact
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /2019-01-01/contact-group/{id}/relationships/contact
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /2019-01-01/contact-group/{id}/relationships/contact
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-01-01/job-reference/{id}/relationships/message
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /2019-01-01/job-reference/{id}/relationships/message
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-01-01/job-reference/{id}/relationships/team
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /2019-01-01/job-reference/{id}/relationships/team
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /2019-01-01/job-reference/{id}/relationships/team
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /2019-01-01/job-reference/{id}/relationships/user
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-01-01/keyword/{id}/relationships/user
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /2019-01-01/keyword/{id}/relationships/user
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-01-01/message/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-01-01/message/{id}/relationships/assignment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /2019-01-01/message/{id}/relationships/category-tag
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /2019-01-01/message/{id}/relationships/category-tag
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /2019-01-01/message/{id}/relationships/category-tag
operation_count: 162
overview: 'SEDNA exposes 162 API operations that an AI agent could call, of which 81 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 81 read, 35 write, 42 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SEDNA
provider_slug: sedna
slug: sedna-agentic-access
source_filename: sedna-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/sedna-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 162\n  by_action_class:\n    acting: 81\n    connected: 81\n  by_consequence:\n    write: 35\n    read: 81\n    physical: 42\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /2019-01-01/category-tag\n  method: post\n  operationId: createCategoryTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/category-tag\n  method: get\n  operationId: getCategoryTags\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/category-tag/{id}\n  method: delete\n  operationId: deleteCategoryTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/category-tag/{id}\n  method: get\n  operationId: getCategoryTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/category-tag/{id}\n  method: patch\n  operationId: updateCategoryTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/category-tag/{id}/message\n  method: get\n  operationId: getMessagesWithCategoryTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/category-tag/{id}/messageV2\n  method: get\n  operationId: getMessagesWithCategoryTagV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/category-tag/{id}/relationships/message\n  method: post\n  operationId: addCategoryTagToMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/category-tag/{id}/relationships/message\n  method: get\n  operationId: getCategoryTagMessageRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/category-tag/{id}/relationships/message\n  method: delete\n  operationId: removeCategoryTagFromMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/category-tag/{id}/relationships/team\n  method: post\n  operationId: addCategoryTagTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/category-tag/{id}/relationships/team\n  method: delete\n  operationId: deleteCategoryTagTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/category-tag/{id}/relationships/team\n  method: get\n  operationId: getCategoryTagTeamRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/category-tag/{id}/relationships/team\n\
  \  method: patch\n  operationId: replaceCategoryTagTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/category-tag/{id}/team\n  method: get\n  operationId: getCategoryTagTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/chartering/vessel\n  method: post\n  operationId: createVessel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /2019-01-01/comment\n  method: get\n  operationId: getComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/company/me\n  method: get\n  operationId: find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/company/me\n  method: patch\n  operationId: patchCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact\n  method: get\n  operationId: getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/contact-group\n  method: post\n  operationId: createContactGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact-group\n  method: get\n  operationId: getContactGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/contact-group/{id}\n  method: delete\n\
  \  operationId: deleteContactGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact-group/{id}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/contact-group/{id}\n  method: patch\n  operationId: updateContactGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact-group/{id}/relationships/contact\n  method: post\n  operationId:\
  \ addContactToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact-group/{id}/relationships/contact\n  method: delete\n  operationId: removeContactFromGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact-group/{id}/relationships/contact\n  method: patch\n  operationId: replaceGroupContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact/{id}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact/{id}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/contact/{id}\n  method: put\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact/{id}/comment\n  method: post\n  operationId: addContactComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact/{id}/comment\n  method: delete\n  operationId: deleteContactComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact/{id}/comment\n  method: get\n  operationId: getContactComments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/contact/{id}/comment\n  method: put\n  operationId: updateContactComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/contact/{id}/relationships/contact-group\n  method: get\n  operationId: getContactGroupRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/contact/{id}/relationships/team\n  method: get\n  operationId: getContactTeamRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/document/{id}\n  method: get\n  operationId: getDocumentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/download/document/{id}\n  method: get\n  operationId: downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/download/message/{id}\n  method: get\n  operationId: downloadMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/download/message/{id}/attachments/zip\n  method: get\n  operationId: downloadAllMessageAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /2019-01-01/download/template/document/{id}\n  method: get\n  operationId: downloadTemplateDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/event\n  method: get\n  operationId: getEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/event/latest\n  method: get\n  operationId: getLatestEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/event/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/event/{id}/category-tag\n  method: get\n  operationId: getEventCategoryTag\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/event/{id}/job-reference\n  method: get\n  operationId: getEventJobReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/event/{id}/message\n  method: get\n  operationId: getEventMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/event/{id}/relationships/category-tag\n  method: get\n  operationId: getEventCategoryTagRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/event/{id}/relationships/job-reference\n  method: get\n  operationId: getEventJobReferenceRelationships\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/event/{id}/relationships/message\n  method: get\n  operationId: getEventMessageRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/job-reference\n  method: post\n  operationId: createJobReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/job-reference\n  method: get\n  operationId: getJobReferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /2019-01-01/job-reference/{id}\n  method: delete\n  operationId: deleteJobReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/job-reference/{id}\n  method: get\n  operationId: getJobReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/job-reference/{id}\n  method: patch\n  operationId: updateJobReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/job-reference/{id}/message\n\
  \  method: get\n  operationId: getMessagesWithJobReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/job-reference/{id}/messageV2\n  method: get\n  operationId: getMessagesWithJobReferenceV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/job-reference/{id}/relationships/message\n  method: post\n  operationId: addJobReferenceToMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/job-reference/{id}/relationships/message\n  method: get\n  operationId:\
  \ getJobReferenceMessageRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/job-reference/{id}/relationships/message\n  method: delete\n  operationId: removeJobReferenceFromMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/job-reference/{id}/relationships/team\n  method: post\n  operationId: addJobReferenceTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/job-reference/{id}/relationships/team\n  method: delete\n  operationId: deleteJobReferenceTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/job-reference/{id}/relationships/team\n  method: get\n  operationId: getJobReferenceTeamRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/job-reference/{id}/relationships/team\n  method: patch\n  operationId: replaceJobReferenceTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/job-reference/{id}/relationships/user\n  method: get\n  operationId: getJobReferenceUserRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/job-reference/{id}/relationships/user\n  method: delete\n  operationId: removeJobReferenceUserRelationships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/keyword\n  method:\
  \ post\n  operationId: createKeyword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/keyword\n  method: get\n  operationId: getKeywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/keyword/{id}\n  method: delete\n  operationId: deleteKeyword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/keyword/{id}\n  method: get\n  operationId: getKeyword\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/keyword/{id}/relationships/user\n  method: post\n  operationId: addKeywordUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/keyword/{id}/relationships/user\n  method: delete\n  operationId: removeKeywordUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message\n\
  \  method: post\n  operationId: createMessageDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/quarantine\n  method: get\n  operationId: listQuarantinedMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/send\n  method: post\n  operationId: sendNewMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}\n\
  \  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/{id}\n  method: patch\n  operationId: updateMessageDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/assignment\n  method: get\n  operationId: getMessageAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/{id}/category-tag\n  method: get\n  operationId: getMessageCategoryTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/{id}/comment\n  method: get\n  operationId: getMessageComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/{id}/document\n  method: post\n  operationId: addDocumentToMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/document\n  method: get\n  operationId: getMessageDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/{id}/job-reference\n  method: get\n  operationId: getMessageJobReferences\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/{id}/quarantine\n  method: patch\n  operationId: quarantineMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/quarantine/event\n  method: get\n  operationId: getMessageQuarantineEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/{id}/relationships/assignment\n  method: post\n  operationId: addAssignments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/relationships/category-tag\n  method: post\n  operationId: addMessageCategoryTags\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/relationships/category-tag\n  method: get\n  operationId: getMessageCategoryTagRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/{id}/relationships/category-tag\n  method: delete\n  operationId:\
  \ removeMessageCategoryTags\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/relationships/category-tag\n  method: patch\n  operationId: replaceMessageCategoryTags\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/relationships/document\n  method: get\n  operationId: getMessageDocumentRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/{id}/relationships/job-reference\n  method: post\n  operationId: addMessageJobReferences\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/relationships/job-reference\n  method: delete\n  operationId: deleteMessageJobReferences\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/relationships/job-reference\n\
  \  method: get\n  operationId: getMessageJobReferenceRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/{id}/relationships/job-reference\n  method: patch\n  operationId: replaceMessageJobReferences\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/relationships/team\n  method: post\n  operationId: addMessageTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/relationships/team\n  method: delete\n  operationId: deleteMessageTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/relationships/team\n  method: get\n  operationId: getMessageTeamRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2019-01-01/message/{id}/relationships/team\n  method: patch\n  operationId: replaceMessageTeams\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/send\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2019-01-01/message/{id}/send\n  method: patch\n  operationId: updateAndSendMessagePatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalatio\n\n# --- truncated at 32 KB (50 KB total) ---\n#\
  \ Full source: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/agentic-access/sedna-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/agentic-access/sedna-agentic-access.yml
summary_line: 162 operations · 81 acting · 4 human-in-the-loop
tags:
- Company
- Shipping
- Maritime
- Email
- Communications
- Workflow
- Commodity Trading
- Logistics
- Messaging
---
