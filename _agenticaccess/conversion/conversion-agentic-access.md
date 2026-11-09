---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 6
api_specs:
- filename: conversion-audiences-api-openapi.yml
  format: yaml
  label: Conversion Audiences API
  slug: conversion-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-audiences-api-openapi.yml
- filename: conversion-campaigns-api-openapi.yml
  format: yaml
  label: Conversion Campaigns API
  slug: conversion-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-campaigns-api-openapi.yml
- filename: conversion-contacts-api-openapi.yml
  format: yaml
  label: Conversion Contacts API
  slug: conversion-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-contacts-api-openapi.yml
- filename: conversion-custom-objects-api-openapi.yml
  format: yaml
  label: Conversion Custom Objects API
  slug: conversion-custom-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-custom-objects-api-openapi.yml
- filename: conversion-events-api-openapi.yml
  format: yaml
  label: Conversion Events API
  slug: conversion-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-events-api-openapi.yml
- filename: conversion-exports-api-openapi.yml
  format: yaml
  label: Conversion Exports API
  slug: conversion-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-exports-api-openapi.yml
- filename: conversion-fields-api-openapi.yml
  format: yaml
  label: Conversion Fields API
  slug: conversion-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-fields-api-openapi.yml
- filename: conversion-forms-api-openapi.yml
  format: yaml
  label: Conversion Forms API
  slug: conversion-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-forms-api-openapi.yml
- filename: conversion-full-delete-api-openapi.yml
  format: yaml
  label: Conversion Full Delete API
  slug: conversion-full-delete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-full-delete-api-openapi.yml
- filename: conversion-workflows-api-openapi.yml
  format: yaml
  label: Conversion Workflows API
  slug: conversion-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-workflows-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Conversion Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/fields/relationships
operation_count: 29
overview: 'Conversion exposes 29 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 22 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Conversion
provider_slug: conversion
slug: conversion-agentic-access
source_filename: conversion-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/conversion-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 23\n    connected: 6\n  by_consequence:\n    write: 22\n    read: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/contacts\n  method: post\n  operationId: upsertContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/contacts\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/contacts/batch\n  method: post\n  operationId: batchUpsertContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/events\n  method: post\n  operationId: trackEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/events/batch\n  method: post\n  operationId: batchTrackEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fields\n  method: get\n  operationId: listFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/fields\n  method: post\n  operationId: createField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fields/relationships\n  method: post\n  operationId: createRelationshipField\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/custom-objects/{customObjectId}/records/batch\n  method: post\n  operationId: batchUpsertCustomObjectRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/forms\n  method: get\n  operationId: listForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/forms/{formId}\n  method: get\n  operationId: getForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workflows/{workflowId}/trigger\n  method: post\n  operationId:\
  \ triggerWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/audiences/{audienceId}/contacts\n  method: post\n  operationId: addContactToAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/audiences/{audienceId}/contacts\n  method: delete\n  operationId: removeContactFromAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /v2/campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns/{campaignId}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/campaigns/{campaignId}/members\n  method: post\n  operationId: addCampaignMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/campaigns/{campaignId}/members/batch\n  method: post\n  operationId: batchAddCampaignMembers\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/exports/contacts\n  method: post\n  operationId: exportContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/exports/email-events\n  method: post\n  operationId: exportEmailEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/exports/custom-events\n  method:\
  \ post\n  operationId: exportCustomEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/exports/contact-events\n  method: post\n  operationId: exportContactEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/exports/campaigns\n  method: post\n  operationId: exportCampaigns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/exports/campaign-types\n  method: post\n  operationId: exportCampaignTypes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/exports/workflows\n  method: post\n  operationId: exportWorkflows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/exports/audiences\n  method: post\n  operationId: exportAudiences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/exports/audience-members\n  method: post\n  operationId: exportAudienceMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/exports/touchpoints\n  method: post\n  operationId: exportTouchpoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/full-delete\n  method: post\n  operationId: fullDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/conversion/agentic-access/conversion-agentic-access.yml
summary_line: 29 operations · 23 acting
tags:
- Marketing
- Automation
- Artificial Intelligence
- B2B
- Software-as-a-Service
- Platform
---
