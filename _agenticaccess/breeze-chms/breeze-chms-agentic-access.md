---
acting_count: 0
action_class_counts:
  connected: 47
api_specs:
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze People API
  slug: breeze-chms-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Tags API
  slug: breeze-chms-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Events API
  slug: breeze-chms-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Check-Ins and Attendance API
  slug: breeze-chms-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Giving and Contributions API
  slug: breeze-chms-giving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Funds API
  slug: breeze-chms-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Pledges API
  slug: breeze-chms-pledges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Forms API
  slug: breeze-chms-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Volunteers API
  slug: breeze-chms-volunteers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
- filename: breeze-chms-openapi.yml
  format: yaml
  label: Breeze Account API
  slug: breeze-chms-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-openapi.yml
consequence_counts:
  read: 47
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Breeze Chms Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 47
overview: 'Breeze ChMS exposes 47 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 47 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Breeze ChMS
provider_slug: breeze-chms
slug: breeze-chms-agentic-access
source_filename: breeze-chms-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/breeze-chms-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 47\n  by_consequence:\n    read: 47\n  human_in_the_loop_required: 0\noperations:\n- path: /people\n  method: get\n  operationId: listPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{person_id}\n  method: get\n  operationId: getPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/add\n  method: get\n  operationId: addPerson\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/update\n  method: get\n  operationId: updatePerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/delete\n  method: get\n  operationId: deletePerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: get\n  operationId: listProfileFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /families/create\n  method: get\n  operationId: createFamily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /families/add\n\
  \  method: get\n  operationId: addToFamily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /families/remove\n  method: get\n  operationId: removeFromFamily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/list_tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/list_folders\n  method: get\n  operationId: listTagFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/add_tag\n  method: get\n  operationId: addTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/add_tag_folder\n  method: get\n  operationId: addTagFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/delete_tag\n  method: get\n  operationId: deleteTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/delete_tag_folder\n  method: get\n  operationId: deleteTagFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/assign\n  method: get\n  operationId: assignTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/unassign\n  method: get\n  operationId: unassignTag\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/list_event\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/calendars/list\n  method: get\n  operationId: listCalendars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/add\n\
  \  method: get\n  operationId: addEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/delete\n  method: get\n  operationId: deleteEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/attendance/add\n  method: get\n  operationId: addAttendance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/attendance/delete\n  method: get\n  operationId: deleteAttendance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/attendance/list\n  method: get\n  operationId: listAttendance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/attendance/eligible\n  method: get\n  operationId: listEligible\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /giving/list\n  method: get\n  operationId: listContributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /giving/add\n  method: get\n  operationId: addContribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /giving/edit\n  method: get\n  operationId: editContribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /giving/delete\n  method: get\n  operationId:\
  \ deleteContribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funds/list\n  method: get\n  operationId: listFunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pledges/list_campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pledges/list_pledges\n  method: get\n  operationId: listPledges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/list_forms\n  method: get\n  operationId: listForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /forms/list_form_fields\n  method: get\n  operationId: listFormFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/list_form_entries\n  method: get\n  operationId: listFormEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/remove_form_entry\n  method: get\n  operationId: removeFormEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volunteers/list\n  method: get\n  operationId: listVolunteers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volunteers/add\n  method: get\n  operationId: addVolunteer\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volunteers/remove\n  method: get\n  operationId: removeVolunteer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volunteers/update\n  method: get\n  operationId: updateVolunteer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volunteers/list_roles\n  method: get\n  operationId: listVolunteerRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volunteers/add_role\n  method: get\n  operationId: addVolunteerRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /volunteers/remove_role\n  method: get\n  operationId: removeVolunteerRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/summary\n  method: get\n  operationId: accountSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/list_log\n  method: get\n  operationId: listAccountLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/agentic-access/breeze-chms-agentic-access.yml
summary_line: 47 operations
tags:
- Church Management
- ChMS
- Nonprofit
- Giving
- Membership
- Events
- Faith
---
