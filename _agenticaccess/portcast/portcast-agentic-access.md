---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: portcast-openapi.yml
  format: yaml
  label: Portcast Container Tracking API
  slug: container-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-openapi.yml
- filename: portcast-openapi.yml
  format: yaml
  label: Portcast Predictive ETA API
  slug: predictive-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-openapi.yml
- filename: portcast-openapi.yml
  format: yaml
  label: Portcast Vessel Schedules API
  slug: vessel-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-openapi.yml
- filename: portcast-openapi.yml
  format: yaml
  label: Portcast Webhooks (Push API)
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-openapi.yml
consequence_counts:
  read: 7
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Portcast Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Portcast exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Portcast
provider_slug: portcast
slug: portcast-agentic-access
source_filename: portcast-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/portcast-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 6\n    connected: 7\n  by_consequence:\n    write: 6\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /bill-of-lading-bookmarks\n  method: post\n  operationId: uploadUsingContainerNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booking\n  method: post\n  operationId: uploadUsingBooking\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bill-of-lading-bookmarks/{bookmark_id}\n  method: delete\n  operationId: archiveBookmark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tracking/bill-of-lading-bookmarks\n  method: get\n  operationId: listTrackingData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracking/bill-of-lading-bookmarks/{bookmark_id}\n  method: get\n  operationId: fetchTrackingData\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracking/bill-of-lading-bookmarks/{bookmark_id}/container_route\n  method: get\n  operationId: getContainerRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracking/bill-of-lading-bookmarks/{bookmark_id}/risks\n  method: get\n  operationId: getContainerRisks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracking/bill-of-lading-bookmarks/{bookmark_id}/import_export_plan\n  method: get\n  operationId: getContainerTerminalData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracking/bill-of-lading-bookmarks/{bookmark_id}/augmentations\n  method: get\n\
  \  operationId: fetchAugmentation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tracking/bill-of-lading-bookmarks/{bookmark_id}/augmentations\n  method: post\n  operationId: uploadAugmentation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tracking/bill-of-lading-bookmarks/{bookmark_id}/augmentations\n  method: put\n  operationId: updateAugmentation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tracking/bill-of-lading-bookmarks/{bookmark_id}/augmentations\n\
  \  method: delete\n  operationId: deleteAugmentation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scac\n  method: get\n  operationId: listCarrierScac\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/agentic-access/portcast-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Supply Chain
- Container Tracking
- Logistics
- Predictive ETA
- Ocean Freight
---
