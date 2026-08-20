---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 10
api_specs:
- filename: emailoctopus-automation-api-openapi.yml
  format: yaml
  label: EmailOctopus Automation API
  slug: emailoctopus-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-automation-api-openapi.yml
- filename: emailoctopus-campaign-api-openapi.yml
  format: yaml
  label: EmailOctopus Campaign API
  slug: emailoctopus-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-campaign-api-openapi.yml
- filename: emailoctopus-contact-api-openapi.yml
  format: yaml
  label: EmailOctopus Contact API
  slug: emailoctopus-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-contact-api-openapi.yml
- filename: emailoctopus-field-api-openapi.yml
  format: yaml
  label: EmailOctopus Field API
  slug: emailoctopus-field-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-field-api-openapi.yml
- filename: emailoctopus-list-api-openapi.yml
  format: yaml
  label: EmailOctopus List API
  slug: emailoctopus-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-list-api-openapi.yml
- filename: emailoctopus-tag-api-openapi.yml
  format: yaml
  label: EmailOctopus Tag API
  slug: emailoctopus-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-tag-api-openapi.yml
consequence_counts:
  read: 10
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Emailoctopus Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'EmailOctopus exposes 25 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: EmailOctopus
provider_slug: emailoctopus
slug: emailoctopus-agentic-access
source_filename: emailoctopus-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/emailoctopus-automation-api-openapi.yml, openapi/emailoctopus-campaign-api-openapi.yml,\n  openapi/emailoctopus-contact-api-openapi.yml, openapi/emailoctopus-field-api-openapi.yml,\n  openapi/emailoctopus-list-api-openapi.yml, openapi/emailoctopus-tag-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    acting: 15\n    connected: 10\n  by_consequence:\n    write: 15\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /automations/{automation_id}/queue\n  method: post\n  operationId: api_automations_automation_idqueue_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns\n  method: get\n  operationId: api_campaigns_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{campaign_id}\n  method: get\n  operationId: api_campaigns_campaign_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{campaign_id}/reports\n  method: get\n  operationId: api_campaigns_campaign_idreports_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{campaign_id}/reports/links\n  method: get\n  operationId: api_campaigns_campaign_idreportslinks_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{campaign_id}/reports/summary\n  method: get\n  operationId: api_campaigns_campaign_idreportssummary_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{list_id}/contacts\n  method: get\n  operationId: api_lists_list_idcontacts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{list_id}/contacts\n  method: put\n  operationId: api_lists_list_idcontacts_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /lists/{list_id}/contacts\n  method: post\n  operationId: api_lists_list_idcontacts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}/contacts/batch\n  method: put\n  operationId: api_lists_list_idcontactsbatch_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}/contacts/{contact_id}\n  method: get\n  operationId: api_lists_list_idcontacts_contact_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{list_id}/contacts/{contact_id}\n  method: put\n  operationId: api_lists_list_idcontacts_contact_id_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}/contacts/{contact_id}\n  method: delete\n  operationId: api_lists_list_idcontacts_contact_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}/fields\n  method: post\n  operationId: api_lists_list_idfields_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}/fields/{tag}\n  method: put\n  operationId: api_lists_list_idfields_tag_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}/fields/{tag}\n  method: delete\n  operationId: api_lists_list_idfields_tag_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /lists\n  method: get\n  operationId: api_lists_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists\n  method: post\n  operationId: api_lists_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}\n  method: get\n  operationId: api_lists_list_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{list_id}\n  method: put\n  operationId: api_lists_list_id_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}\n  method: delete\n  operationId: api_lists_list_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}/tags\n  method: get\n  operationId: api_lists_list_idtags_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{list_id}/tags\n  method: post\n  operationId: api_lists_list_idtags_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}/tags/{tag}\n  method: put\n  operationId: api_lists_list_idtags_tag_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}/tags/{tag}\n  method: delete\n  operationId: api_lists_list_idtags_tag_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/agentic-access/emailoctopus-agentic-access.yml
summary_line: 25 operations · 15 acting
tags:
- Email
- Email Marketing
- Newsletters
- Campaigns
- Automation
- Contacts
- List
- Marketing
- Webhook
- Transactional Email
- Subscriber Management
- Reporting
---
