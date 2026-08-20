---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: fairmarkit-business-units-api-openapi.yml
  format: yaml
  label: Fairmarkit Business Units API
  slug: fairmarkit-business-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-business-units-api-openapi.yml
- filename: fairmarkit-categories-api-openapi.yml
  format: yaml
  label: Fairmarkit Categories API
  slug: fairmarkit-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-categories-api-openapi.yml
- filename: fairmarkit-data-exports-api-openapi.yml
  format: yaml
  label: Fairmarkit Data Exports API
  slug: fairmarkit-data-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-data-exports-api-openapi.yml
- filename: fairmarkit-data-fields-api-openapi.yml
  format: yaml
  label: Fairmarkit Data Fields API
  slug: fairmarkit-data-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-data-fields-api-openapi.yml
- filename: fairmarkit-erp-systems-api-openapi.yml
  format: yaml
  label: Fairmarkit ERP Systems API
  slug: fairmarkit-erp-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-erp-systems-api-openapi.yml
- filename: fairmarkit-event-api-openapi.yml
  format: yaml
  label: Fairmarkit Event API
  slug: fairmarkit-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-event-api-openapi.yml
- filename: fairmarkit-file-attachments-api-openapi.yml
  format: yaml
  label: Fairmarkit File attachments API
  slug: fairmarkit-file-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-file-attachments-api-openapi.yml
- filename: fairmarkit-identity-api-openapi.yml
  format: yaml
  label: Fairmarkit Identity API
  slug: fairmarkit-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-identity-api-openapi.yml
- filename: fairmarkit-price-books-api-openapi.yml
  format: yaml
  label: Fairmarkit Price Books API
  slug: fairmarkit-price-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-price-books-api-openapi.yml
- filename: fairmarkit-purchase-orders-api-openapi.yml
  format: yaml
  label: Fairmarkit Purchase Orders API
  slug: fairmarkit-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-purchase-orders-api-openapi.yml
- filename: fairmarkit-requests-api-openapi.yml
  format: yaml
  label: Fairmarkit Requests API
  slug: fairmarkit-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-requests-api-openapi.yml
- filename: fairmarkit-responses-api-openapi.yml
  format: yaml
  label: Fairmarkit Responses API
  slug: fairmarkit-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-responses-api-openapi.yml
- filename: fairmarkit-rfp-api-openapi.yml
  format: yaml
  label: Fairmarkit RFP API
  slug: fairmarkit-rfp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-rfp-api-openapi.yml
- filename: fairmarkit-rfq-api-openapi.yml
  format: yaml
  label: Fairmarkit RFQ API
  slug: fairmarkit-rfq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-rfq-api-openapi.yml
- filename: fairmarkit-schema-api-openapi.yml
  format: yaml
  label: Fairmarkit Schema API
  slug: fairmarkit-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-schema-api-openapi.yml
- filename: fairmarkit-supplier-api-openapi.yml
  format: yaml
  label: Fairmarkit Supplier API
  slug: fairmarkit-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-supplier-api-openapi.yml
- filename: fairmarkit-uom-api-openapi.yml
  format: yaml
  label: Fairmarkit UOM API
  slug: fairmarkit-uom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-uom-api-openapi.yml
- filename: fairmarkit-user-profiles-api-openapi.yml
  format: yaml
  label: Fairmarkit User Profiles API
  slug: fairmarkit-user-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/openapi/fairmarkit-user-profiles-api-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fairmarkit Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Fairmarkit exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fairmarkit
provider_slug: fairmarkit
slug: fairmarkit-agentic-access
source_filename: fairmarkit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/fairmarkit-supplier-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 2\n    connected: 3\n  by_consequence:\n    write: 2\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /services/supplier-public-api/api/v1/requests/{request_id}/reject/\n  method: post\n  operationId: reject_request-Requests_Requests_Requests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/supplier-public-api/api/v1/requests/{request_id}/response/\n\
  \  method: get\n  operationId: get_request_response-Requests_Requests_Requests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/supplier-public-api/api/v1/requests/{request_id}/\n  method: get\n  operationId: get_request-Requests_Requests_Requests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/supplier-public-api/api/v1/requests/{request_id}/submit/\n  method: post\n  operationId: submit_response-Requests_Requests_Requests\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/supplier-public-api/api/v1/requests/\n  method:\
  \ get\n  operationId: get_requests-Requests_Requests_Requests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fairmarkit/refs/heads/main/agentic-access/fairmarkit-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Company
- Procurement
- Sourcing
- Supply Chain
- Purchasing
- Suppliers
- RFQ
- RFP
- Spend Management
- Webhook
---
