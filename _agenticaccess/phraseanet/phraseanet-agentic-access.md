---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 20
api_specs:
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Records API
  slug: phraseanet-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Databoxes and Collections API
  slug: phraseanet-databoxes-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Metadata API
  slug: phraseanet-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Search API
  slug: phraseanet-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Stories API
  slug: phraseanet-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Baskets API
  slug: phraseanet-baskets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Feeds API
  slug: phraseanet-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
- filename: phraseanet-openapi.yml
  format: yaml
  label: Phraseanet Account API
  slug: phraseanet-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/openapi/phraseanet-openapi.yml
consequence_counts:
  read: 20
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Phraseanet Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 34
overview: 'Phraseanet exposes 34 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Phraseanet
provider_slug: phraseanet
slug: phraseanet-agentic-access
source_filename: phraseanet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/phraseanet-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 20\n    acting: 14\n  by_consequence:\n    read: 20\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /databoxes/list\n  method: get\n  operationId: listDataboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /databoxes/{databox_id}/collections\n  method:\
  \ get\n  operationId: listDataboxCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /databoxes/{databox_id}/status\n  method: get\n  operationId: getDataboxStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /databoxes/{databox_id}/metadatas\n  method: get\n  operationId: getDataboxMetadatas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /databoxes/{databox_id}/termsOfUse\n  method: get\n  operationId: getDataboxTermsOfUse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /records/add\n  method: post\n  operationId: addRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /records/{databox_id}/{record_id}\n  method: get\n  operationId: getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /records/{databox_id}/{record_id}/caption\n  method: get\n  operationId: getRecordCaption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /records/{databox_id}/{record_id}/metadatas\n  method: get\n  operationId: getRecordMetadatas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /records/{databox_id}/{record_id}/setmetadatas\n  method: post\n  operationId: setRecordMetadatas\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /records/{databox_id}/{record_id}/status\n  method: get\n  operationId: getRecordStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /records/{databox_id}/{record_id}/setstatus\n  method: post\n  operationId:\
  \ setRecordStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /records/{databox_id}/{record_id}/embed\n  method: get\n  operationId: getRecordEmbed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /records/{databox_id}/{record_id}/related\n  method: get\n  operationId: getRecordRelated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /records/{databox_id}/{record_id}/setcollection\n  method: post\n  operationId: setRecordCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /records/{databox_id}/{record_id}/delete\n  method: post\n  operationId: deleteRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/add\n  method: post\n  operationId: addStory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{databox_id}/{story_id}\n  method: get\n  operationId: getStory\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories/{databox_id}/{story_id}/addrecords\n  method: post\n  operationId: addRecordsToStory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{databox_id}/{story_id}/delrecords\n  method: post\n  operationId: removeRecordsFromStory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{databox_id}/{story_id}/setcover\n  method: post\n  operationId: setStoryCover\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/list\n  method: get\n  operationId: listBaskets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /baskets/add\n  method: post\n  operationId: addBasket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/{basket_id}/content\n  method: get\n  operationId: getBasketContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /baskets/{basket_id}/setname\n  method: post\n  operationId: setBasketName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/{basket_id}/setdescription\n  method: post\n  operationId: setBasketDescription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /baskets/{basket_id}/delete\n  method: post\n  operationId: deleteBasket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/list\n  method: get\n  operationId: listFeeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/{feed_id}/content\n  method: get\n  operationId: getFeedContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/aggregated/content\n  method: get\n  operationId: getAggregatedFeedContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quarantine/list\n  method: get\n  operationId: listQuarantine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /quarantine/{quarantine_item_id}\n  method: get\n  operationId: getQuarantineItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phraseanet/refs/heads/main/agentic-access/phraseanet-agentic-access.yml
summary_line: 34 operations · 14 acting
tags:
- Digital Asset Management
- DAM
- Media
- Metadata
- Open Source
- Search
---
