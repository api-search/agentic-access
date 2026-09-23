---
acting_count: 58
action_class_counts:
  acting: 58
api_specs:
- filename: teamleader-contacts-api-openapi.yml
  format: yaml
  label: Teamleader Contacts API
  slug: teamleader-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-contacts-api-openapi.yml
- filename: teamleader-daysoff-api-openapi.yml
  format: yaml
  label: Teamleader Daysoff API
  slug: teamleader-daysoff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-daysoff-api-openapi.yml
- filename: teamleader-deals-api-openapi.yml
  format: yaml
  label: Teamleader Deals API
  slug: teamleader-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-deals-api-openapi.yml
- filename: teamleader-expenses-api-openapi.yml
  format: yaml
  label: Teamleader Expenses API
  slug: teamleader-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-expenses-api-openapi.yml
- filename: teamleader-files-api-openapi.yml
  format: yaml
  label: Teamleader Files API
  slug: teamleader-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-files-api-openapi.yml
- filename: teamleader-invoices-api-openapi.yml
  format: yaml
  label: Teamleader Invoices API
  slug: teamleader-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-invoices-api-openapi.yml
- filename: teamleader-leveltwoareas-api-openapi.yml
  format: yaml
  label: Teamleader Leveltwoareas API
  slug: teamleader-leveltwoareas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-leveltwoareas-api-openapi.yml
- filename: teamleader-lostreasons-api-openapi.yml
  format: yaml
  label: Teamleader Lostreasons API
  slug: teamleader-lostreasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-lostreasons-api-openapi.yml
- filename: teamleader-tasks-api-openapi.yml
  format: yaml
  label: Teamleader Tasks API
  slug: teamleader-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-tasks-api-openapi.yml
- filename: teamleader-tickets-api-openapi.yml
  format: yaml
  label: Teamleader Tickets API
  slug: teamleader-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-tickets-api-openapi.yml
- filename: teamleader-ticketstatus-api-openapi.yml
  format: yaml
  label: Teamleader Ticketstatus API
  slug: teamleader-ticketstatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-ticketstatus-api-openapi.yml
- filename: teamleader-timers-api-openapi.yml
  format: yaml
  label: Teamleader Timers API
  slug: teamleader-timers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-timers-api-openapi.yml
- filename: teamleader-useravailability-api-openapi.yml
  format: yaml
  label: Teamleader Useravailability API
  slug: teamleader-useravailability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-useravailability-api-openapi.yml
- filename: teamleader-payment-methods-api-openapi.yml
  format: yaml
  label: Teamleader Payment Methods API
  slug: teamleader-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/openapi/teamleader-payment-methods-api-openapi.yml
consequence_counts:
  physical: 10
  write: 48
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Teamleader Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices.book
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices.copy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices.delete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices.download
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices.draft
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices.info
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices.list
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices.update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoices.updateBooked
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentMethods.list
operation_count: 58
overview: 'Teamleader exposes 58 API operations that an AI agent could call, of which 58 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 48 write and 10 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Teamleader
provider_slug: teamleader
slug: teamleader-agentic-access
source_filename: teamleader-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: generated\nsource: openapi/teamleader-openapi-generated.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 58\n  by_action_class:\n    acting: 58\n  by_consequence:\n    write: 48\n    physical: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /contacts.add\n  method: post\n  operationId: post_contacts_add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts.delete\n  method: post\n  operationId: post_contacts_delete\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts.info\n  method: post\n  operationId: post_contacts_info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts.linkToCompany\n  method: post\n  operationId: post_contacts_linkToCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts.list\n  method: post\n  operationId:\
  \ post_contacts_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts.tag\n  method: post\n  operationId: post_contacts_tag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts.unlinkFromCompany\n  method: post\n  operationId: post_contacts_unlinkFromCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /contacts.untag\n  method: post\n  operationId: post_contacts_untag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts.update\n  method: post\n  operationId: post_contacts_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts.updateCompanyLink\n  method: post\n  operationId: post_contacts_updateCompanyLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts.uploadAvatar\n  method: post\n  operationId: post_contacts_uploadAvatar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /daysOff.bulkDelete\n  method: post\n  operationId: post_daysOff_bulkDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deals.create\n  method: post\n  operationId: post_deals_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deals.delete\n  method: post\n  operationId: post_deals_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deals.info\n  method: post\n  operationId: post_deals_info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deals.list\n  method: post\n  operationId: post_deals_list\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deals.lose\n  method: post\n  operationId: post_deals_lose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deals.move\n  method: post\n  operationId: post_deals_move\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deals.update\n  method: post\n  operationId: post_deals_update\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deals.win\n  method: post\n  operationId: post_deals_win\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expenses.list\n  method: post\n  operationId: post_expenses_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files.delete\n  method: post\n  operationId:\
  \ post_files_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files.download\n  method: post\n  operationId: post_files_download\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files.info\n  method: post\n  operationId: post_files_info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /files.list\n  method: post\n  operationId: post_files_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files.upload\n  method: post\n  operationId: post_files_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices.book\n  method: post\n  operationId: post_invoices_book\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices.copy\n  method: post\n  operationId: post_invoices_copy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices.delete\n  method: post\n  operationId: post_invoices_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices.download\n  method: post\n  operationId: post_invoices_download\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices.draft\n  method: post\n  operationId: post_invoices_draft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices.info\n  method: post\n  operationId: post_invoices_info\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices.list\n  method: post\n  operationId: post_invoices_list\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices.update\n  method: post\n  operationId: post_invoices_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices.updateBooked\n  method: post\n  operationId:\
  \ post_invoices_updateBooked\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /levelTwoAreas.list\n  method: post\n  operationId: post_levelTwoAreas_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lostReasons.list\n  method: post\n  operationId: post_lostReasons_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentMethods.list\n  method: post\n  operationId: post_paymentMethods_list\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks.complete\n  method: post\n  operationId: post_tasks_complete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks.create\n  method: post\n  operationId: post_tasks_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks.delete\n  method: post\n  operationId: post_tasks_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks.info\n  method: post\n  operationId: post_tasks_info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks.list\n  method: post\n  operationId: post_tasks_list\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks.reopen\n  method: post\n  operationId: post_tasks_reopen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks.schedule\n  method: post\n  operationId: post_tasks_schedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks.update\n  method: post\n  operationId: post_tasks_update\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ticketStatus.list\n  method: post\n  operationId: post_ticketStatus_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets.addInternalMessage\n  method: post\n  operationId: post_tickets_addInternalMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /tickets.addReply\n  method: post\n  operationId: post_tickets_addReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets.create\n  method: post\n  operationId: post_tickets_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets.getMessage\n  method: post\n  operationId: post_tickets_getMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets.importMessage\n  method: post\n  operationId: post_tickets_importMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets.info\n  method: post\n  operationId: post_tickets_info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets.list\n  method: post\n  operationId: post_tickets_list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets.listMessages\n  method: post\n  operationId: post_tickets_listMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets.update\n  method: post\n  operationId: post_tickets_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timers.update\n  method: post\n  operationId: post_timers_update\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userAvailability.daily\n  method: post\n  operationId: post_userAvailability_daily\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/agentic-access/teamleader-agentic-access.yml
summary_line: 58 operations · 58 acting
tags:
- CRM
- Invoicing
- Project Management
- Software-as-a-Service
- SME
---
