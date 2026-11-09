---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 15
api_specs:
- filename: wholechain-connect-api-openapi.yml
  format: yaml
  label: Wholechain Connect API
  slug: wholechain-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-connect-api-openapi.yml
- filename: wholechain-edi-api-openapi.yml
  format: yaml
  label: Wholechain Edi API
  slug: wholechain-edi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-edi-api-openapi.yml
- filename: wholechain-epcis-interface-api-openapi.yml
  format: yaml
  label: Wholechain EPCIS Interface API
  slug: wholechain-epcis-interface-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-epcis-interface-api-openapi.yml
- filename: wholechain-epcis-legacy-interface-api-openapi.yml
  format: yaml
  label: Wholechain EPCIS Legacy Interface API
  slug: wholechain-epcis-legacy-interface-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-epcis-legacy-interface-api-openapi.yml
- filename: wholechain-events-api-openapi.yml
  format: yaml
  label: Wholechain Events API
  slug: wholechain-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-events-api-openapi.yml
- filename: wholechain-externaloauth-api-openapi.yml
  format: yaml
  label: Wholechain External O Auth API
  slug: wholechain-externaloauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-externaloauth-api-openapi.yml
- filename: wholechain-health-api-openapi.yml
  format: yaml
  label: Wholechain Health API
  slug: wholechain-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wholechain/openapi/wholechain-health-api-openapi.yml
consequence_counts:
  physical: 6
  read: 15
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wholechain Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Integration/Documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /Integration/PurchaseOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Integration/PurchaseOrder/review
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Integration/PurchaseOrder/share
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Integration/PurchaseOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Integration/PurchaseOrders/upload
operation_count: 34
overview: 'Wholechain exposes 34 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 13 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wholechain
provider_slug: wholechain
slug: wholechain-agentic-access
source_filename: wholechain-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/wholechain-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    acting: 19\n    connected: 15\n  by_consequence:\n    write: 13\n    read: 15\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /Integration\n  method: post\n  operationId: XML\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/Events\n  method: post\n  operationId: ProcessEvents\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/Events/async\n  method: post\n  operationId: EnqueueEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/Events/{eventId}\n  method: delete\n  operationId: DeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/Locations\n  method: post\n\
  \  operationId: ProcessLocations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/Locations\n  method: get\n  operationId: ListLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Integration/Location\n  method: put\n  operationId: UpdateLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/Location/{locationId}\n  method: get\n  operationId: GetLocation\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Integration/PurchaseOrder\n  method: get\n  operationId: GetPurchaseOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Integration/PurchaseOrder\n  method: put\n  operationId: UpdatePurchaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/Products\n  method: post\n  operationId: ProcessProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/Products\n  method: get\n  operationId: GetPaginatedProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Integration/Product\n  method: put\n  operationId: UpdateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/files/notification\n  method: post\n  operationId: NotifyNewFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/PackingList\n  method: post\n  operationId: ProcessPackingList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/Jobs\n  method: get\n  operationId: GetJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Integration/Inventory\n  method: get\n  operationId: GetInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Integration/PurchaseOrders\n  method: post\n  operationId: ProcessPurchaseOrders\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/Documents\n  method: post\n  operationId: UploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/PurchaseOrder/review\n  method: post\n  operationId: ReviewPurchaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/PurchaseOrder/share\n  method: post\n  operationId: SharePurchaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Integration/PurchaseOrders/upload\n  method: post\n  operationId: UploadPurchaseOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /epcis/Capture\n\
  \  method: post\n  operationId: Capture\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /epcis/Capture\n  method: get\n  operationId: ListCaptureStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /epcis/Capture/{captureId}\n  method: get\n  operationId: GetCaptureStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /epcis\n  method: get\n  operationId: EpcisQueryInterface\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gdst/{gdstVersion}/epcis/events\n\
  \  method: get\n  operationId: EpcisQueryInterface\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /epcis/Events\n  method: get\n  operationId: EpcisQueryInterface\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /epcis/Queries/SimpleEventQuery\n  method: post\n  operationId: SimpleEventQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Edi/files/notification\n  method: post\n  operationId: NotifyNewEdiFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /epcis/Events/details\n  method: get\n  operationId: ListEventDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration/oauth/login\n  method: get\n  operationId: Login\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integration/oauth/callback\n  method: get\n  operationId: Callback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Health\n  method: get\n  operationId: GetHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://artifacts.apis.io/wholechain/agentic-access/wholechain-agentic-access.yml
summary_line: 34 operations · 19 acting
tags:
- Company
- Supply Chain
- Traceability
- Blockchain
- Food Safety
- Compliance
- GS1
- Logistics
---
