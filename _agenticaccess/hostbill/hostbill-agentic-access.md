---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: hostbill-accounts-api-openapi.yml
  format: yaml
  label: HostBill Accounts API
  slug: hostbill-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-accounts-api-openapi.yml
- filename: hostbill-admin-api-openapi.yml
  format: yaml
  label: HostBill Admin API
  slug: hostbill-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-admin-api-openapi.yml
- filename: hostbill-clients-api-openapi.yml
  format: yaml
  label: HostBill Clients API
  slug: hostbill-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-clients-api-openapi.yml
- filename: hostbill-domains-api-openapi.yml
  format: yaml
  label: HostBill Domains API
  slug: hostbill-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-domains-api-openapi.yml
- filename: hostbill-invoices-api-openapi.yml
  format: yaml
  label: HostBill Invoices API
  slug: hostbill-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-invoices-api-openapi.yml
- filename: hostbill-orders-api-openapi.yml
  format: yaml
  label: HostBill Orders API
  slug: hostbill-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-orders-api-openapi.yml
- filename: hostbill-tickets-api-openapi.yml
  format: yaml
  label: HostBill Tickets API
  slug: hostbill-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-tickets-api-openapi.yml
- filename: hostbill-transactions-api-openapi.yml
  format: yaml
  label: HostBill Transactions API
  slug: hostbill-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/openapi/hostbill-transactions-api-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hostbill Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'HostBill exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HostBill
provider_slug: hostbill
slug: hostbill-agentic-access
source_filename: hostbill-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/hostbill-accounts-api-openapi.yml, openapi/hostbill-admin-api-openapi.yml, openapi/hostbill-clients-api-openapi.yml,\n  openapi/hostbill-domains-api-openapi.yml, openapi/hostbill-invoices-api-openapi.yml, openapi/hostbill-orders-api-openapi.yml,\n  openapi/hostbill-tickets-api-openapi.yml, openapi/hostbill-transactions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 2\n    connected: 6\n  by_consequence:\n    write: 2\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /admin/api.php#addAccount\n  method: post\n  operationId: addAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api.php\n  method: post\n  operationId: callApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/api.php#getClients\n  method: post\n  operationId: getClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api.php#getDomains\n  method: post\n  operationId: getDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api.php#getInvoices\n\
  \  method: post\n  operationId: getInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api.php#getOrders\n  method: post\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api.php#getTickets\n  method: post\n  operationId: getTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/api.php#getTransactions\n  method: post\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hostbill/refs/heads/main/agentic-access/hostbill-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Automation
- Billing
- Domain Registration
- Web Hosting
---
