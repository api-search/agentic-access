---
acting_count: 148
action_class_counts:
  acting: 148
  connected: 189
api_specs:
- filename: university-of-geneva-yareta.yaml
  format: yaml
  label: Yareta Research Data API
  slug: yareta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-geneva/refs/heads/main/openapi/university-of-geneva-yareta.yaml
consequence_counts:
  physical: 71
  read: 189
  write: 77
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: University Of Geneva Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /access/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /access/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /access/orders/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /access/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /access/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /access/orders/{id}/put-in-error
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /access/orders/{id}/resume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /access/orders/{id}/save
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /access/orders/{id}/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /access/orders/{parentid}/aip
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /access/orders/{parentid}/aip
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /access/orders/{parentid}/aip/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /access/orders/{parentid}/aip/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /access/orders/{parentid}/dip
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /access/orders/{parentid}/dip
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /access/orders/{parentid}/dip/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /access/orders/{parentid}/dip/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ingest/sip/{id}/upload
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /preingest/deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /preingest/deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /preingest/deposits/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /preingest/deposits/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /preingest/deposits/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /preingest/deposits/{id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /preingest/deposits/{id}/approve-submission-agreement
operation_count: 337
overview: 'University of Geneva exposes 337 API operations that an AI agent could call, of which 148 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 189 read, 77 write, and 71 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: University of Geneva
provider_slug: university-of-geneva
slug: university-of-geneva-agentic-access
source_filename: university-of-geneva-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/university-of-geneva-yareta.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 337\n  by_action_class:\n    connected: 189\n    acting: 148\n  by_consequence:\n    read: 189\n    write: 77\n    physical: 71\n  human_in_the_loop_required: 0\noperations:\n- path: /oai-info/oai-sets\n  method: get\n  operationId: oai-info_oai-sets_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oai-info/oai-sets\n  method: post\n  operationId: oai-info_oai-sets_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oai-info/oai-sets\n  method: delete\n  operationId: oai-info_oai-sets_deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oai-info/oai-sets/search\n  method: get\n  operationId: oai-info_oai-sets_search_advancedSearch_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oai-info/oai-sets/search\n  method: post\n  operationId: oai-info_oai-sets_search_advancedSearch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oai-info/oai-provider/oai\n  method: get\n  operationId: oai-info_oai-provider_oai_process\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oai-info/oai-provider/oai\n  method: post\n  operationId: oai-info_oai-provider_oai_processPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oai-info/oai-metadata-prefixes\n  method: get\n  operationId: oai-info_oai-metadata-prefixes_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /oai-info/oai-metadata-prefixes\n  method: post\n  operationId: oai-info_oai-metadata-prefixes_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oai-info/oai-metadata-prefixes\n  method: delete\n  operationId: oai-info_oai-metadata-prefixes_deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oai-info/oai-metadata-prefixes/search\n  method: get\n  operationId: oai-info_oai-metadata-prefixes_search_advancedSearch_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oai-info/oai-metadata-prefixes/search\n  method: post\n  operationId: oai-info_oai-metadata-prefixes_search_advancedSearch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/refresh/{aipId}\n  method: post\n  operationId: access_refresh_by_id_refresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/private-metadata/{aipId}/prepare-download\n  method: post\n  operationId: access_private-metadata_by_id_prepare-download\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/private-metadata/search\n  method: get\n  operationId: access_private-metadata_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/private-metadata/search\n  method: post\n  operationId: access_private-metadata_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders\n  method: get\n  operationId: access_orders_list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/orders\n  method: post\n  operationId: access_orders_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders\n  method: delete\n  operationId: access_orders_deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{parentid}/dip\n  method: get\n\
  \  operationId: access_orders_by_id_dip_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/orders/{parentid}/dip\n  method: post\n  operationId: access_orders_by_id_dip_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{parentid}/dip\n  method: delete\n  operationId: access_orders_by_id_dip_deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{parentid}/aip\n  method: get\n  operationId: access_orders_by_id_aip_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/orders/{parentid}/aip\n  method: post\n  operationId: access_orders_by_id_aip_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{parentid}/aip\n  method: delete\n  operationId: access_orders_by_id_aip_deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n   \
  \   exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{id}/submit\n  method: post\n  operationId: access_orders_by_id_submit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{id}/save\n  method: post\n  operationId: access_orders_by_id_save\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /access/orders/{id}/resume\n  method: post\n  operationId: access_orders_by_id_resume\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{id}/put-in-error\n  method: post\n  operationId: access_orders_by_id_put-in-error\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/search\n  method: get\n  operationId: access_orders_search_advancedSearch_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/orders/search\n  method: post\n  operationId: access_orders_search_advancedSearch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/metadata/{parentid}/ratings\n  method: get\n  operationId: access_metadata_by_id_ratings_getArchiveUserRating\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/metadata/{parentid}/ratings\n  method: post\n  operationId: access_metadata_by_id_ratings_create\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/metadata/{parentid}/ratings\n  method: delete\n  operationId: access_metadata_by_id_ratings_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/metadata/{parentid}/ratings\n  method: patch\n  operationId: access_metadata_by_id_ratings_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /access/metadata/{aipId}/prepare-download\n  method: post\n  operationId: access_metadata_by_id_prepare-download\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/metadata/search\n  method: get\n  operationId: access_metadata_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/metadata/search\n  method: post\n  operationId: access_metadata_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /access/dip\n  method: get\n  operationId: access_dip_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/dip\n  method: post\n  operationId: access_dip_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip\n  method: delete\n  operationId: access_dip_deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{parentid}/data\n  method: get\n  operationId:\
  \ access_dip_by_id_data_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/dip/{parentid}/data\n  method: post\n  operationId: access_dip_by_id_data_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{parentid}/data\n  method: delete\n  operationId: access_dip_by_id_data_deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{parentid}/data/{id}/resume\n  method: post\n  operationId:\
  \ access_dip_by_id_data_by_id_resume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{parentid}/aip\n  method: get\n  operationId: access_dip_by_id_aip_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/dip/{parentid}/aip\n  method: post\n  operationId: access_dip_by_id_aip_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{parentid}/aip\n  method: delete\n  operationId: access_dip_by_id_aip_deleteList\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{id}/resume\n  method: post\n  operationId: access_dip_by_id_resume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{id}/put-in-error\n  method: post\n  operationId: access_dip_by_id_put-in-error\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /access/dip/search\n  method: get\n  operationId: access_dip_search_advancedSearch_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/dip/search\n  method: post\n  operationId: access_dip_search_advancedSearch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/all-metadata/{aipId}/prepare-download\n  method: post\n  operationId: access_all-metadata_by_id_prepare-download\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /access/all-metadata/search\n  method: get\n  operationId: access_all-metadata_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/all-metadata/search\n  method: post\n  operationId: access_all-metadata_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip\n  method: get\n  operationId: access_aip_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/aip\n  method: post\n  operationId: access_aip_create\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip\n  method: delete\n  operationId: access_aip_deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip/{parentid}/data\n  method: get\n  operationId: access_aip_by_id_data_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/aip/{parentid}/data\n  method: post\n  operationId: access_aip_by_id_data_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip/{parentid}/data\n  method: delete\n  operationId: access_aip_by_id_data_deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip/{parentid}/data/{id}/resume\n  method: post\n  operationId: access_aip_by_id_data_by_id_resume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip/{parentid}/data/{id}/put-in-error\n\
  \  method: post\n  operationId: access_aip_by_id_data_by_id_put-in-error\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip/{parentid}/aip\n  method: get\n  operationId: access_aip_by_id_aip_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/aip/{parentid}/aip\n  method: post\n  operationId: access_aip_by_id_aip_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip/{parentid}/aip\n\
  \  method: delete\n  operationId: access_aip_by_id_aip_deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip/{id}/resume\n  method: post\n  operationId: access_aip_by_id_resume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip/{id}/put-in-error\n  method: post\n  operationId: access_aip_by_id_put-in-error\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip/search\n  method: get\n  operationId: access_aip_search_advancedSearch_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/aip/search\n  method: post\n  operationId: access_aip_search_advancedSearch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oai-info/oai-sets/{id}\n  method: get\n  operationId: oai-info_oai-sets_by_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oai-info/oai-sets/{id}\n  method: delete\n  operationId: oai-info_oai-sets_by_id_delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oai-info/oai-sets/{id}\n  method: patch\n  operationId: oai-info_oai-sets_by_id_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oai-info/oai-metadata-prefixes/{id}\n  method: get\n  operationId: oai-info_oai-metadata-prefixes_by_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oai-info/oai-metadata-prefixes/{id}\n  method: delete\n  operationId: oai-info_oai-metadata-prefixes_by_id_delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oai-info/oai-metadata-prefixes/{id}\n  method: patch\n  operationId: oai-info_oai-metadata-prefixes_by_id_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{parentid}/dip/{id}\n  method: get\n  operationId: access_orders_by_id_dip_by_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/orders/{parentid}/dip/{id}\n  method: delete\n  operationId:\
  \ access_orders_by_id_dip_by_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{parentid}/dip/{id}\n  method: patch\n  operationId: access_orders_by_id_dip_by_id_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{parentid}/aip/{id}\n  method: get\n  operationId: access_orders_by_id_aip_by_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/orders/{parentid}/aip/{id}\n  method: delete\n  operationId: access_orders_by_id_aip_by_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{parentid}/aip/{id}\n  method: patch\n  operationId: access_orders_by_id_aip_by_id_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{id}\n  method:\
  \ get\n  operationId: access_orders_by_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/orders/{id}\n  method: delete\n  operationId: access_orders_by_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/orders/{id}\n  method: patch\n  operationId: access_orders_by_id_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /access/dip/{parentid}/data/{id}\n  method: get\n  operationId: access_dip_by_id_data_by_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/dip/{parentid}/data/{id}\n  method: delete\n  operationId: access_dip_by_id_data_by_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{parentid}/data/{id}\n  method: patch\n  operationId: access_dip_by_id_data_by_id_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{parentid}/aip/{id}\n  method: get\n  operationId: access_dip_by_id_aip_by_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/dip/{parentid}/aip/{id}\n  method: delete\n  operationId: access_dip_by_id_aip_by_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{parentid}/aip/{id}\n  method: patch\n  operationId: access_dip_by_id_aip_by_id_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{id}\n  method: get\n  operationId: access_dip_by_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/dip/{id}\n  method: delete\n  operationId: access_dip_by_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/dip/{id}\n  method: patch\n  operationId: access_dip_by_id_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /access/aip/{parentid}/data/{id}\n  method: get\n  operationId: access_aip_by_id_data_by_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access/aip/{parentid}/data/{id}\n  method: delete\n  operationId: access_aip_by_id_data_by_id_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access/aip/{parentid}/data/{id}\n  method: patch\n  operationId: access_aip_by_id_data_by_id_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: con\n\n# --- truncated at 32 KB (103 KB total)\
  \ ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/university-of-geneva/refs/heads/main/agentic-access/university-of-geneva-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-geneva/refs/heads/main/agentic-access/university-of-geneva-agentic-access.yml
summary_line: 337 operations · 148 acting
tags:
- Education
- Higher Education
- University
- Open Science
- Research Data
- Institutional Repository
- Switzerland
- Europe
---
