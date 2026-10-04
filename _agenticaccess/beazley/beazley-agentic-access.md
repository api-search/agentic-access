---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 26
api_specs:
- filename: beazley-audit-api-openapi.yml
  format: yaml
  label: Beazley Audit API
  slug: beazley-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-audit-api-openapi.yml
- filename: beazley-check-api-openapi.yml
  format: yaml
  label: Beazley Check API
  slug: beazley-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-check-api-openapi.yml
- filename: beazley-contacts-api-openapi.yml
  format: yaml
  label: Beazley Contacts API
  slug: beazley-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-contacts-api-openapi.yml
- filename: beazley-currencies-api-openapi.yml
  format: yaml
  label: Beazley Currencies API
  slug: beazley-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-currencies-api-openapi.yml
- filename: beazley-cyber-api-openapi.yml
  format: yaml
  label: Beazley Cyber API
  slug: beazley-cyber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-cyber-api-openapi.yml
- filename: beazley-definitions-api-openapi.yml
  format: yaml
  label: Beazley Definitions API
  slug: beazley-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-definitions-api-openapi.yml
- filename: beazley-health-api-openapi.yml
  format: yaml
  label: Beazley Health API
  slug: beazley-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-health-api-openapi.yml
- filename: beazley-lockstate-api-openapi.yml
  format: yaml
  label: Beazley Lockstate API
  slug: beazley-lockstate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-lockstate-api-openapi.yml
- filename: beazley-microsites-api-openapi.yml
  format: yaml
  label: Beazley Microsites API
  slug: beazley-microsites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-microsites-api-openapi.yml
- filename: beazley-organisations-api-openapi.yml
  format: yaml
  label: Beazley Organisations API
  slug: beazley-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-organisations-api-openapi.yml
- filename: beazley-people-api-openapi.yml
  format: yaml
  label: Beazley People API
  slug: beazley-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-people-api-openapi.yml
- filename: beazley-ping-api-openapi.yml
  format: yaml
  label: Beazley Ping API
  slug: beazley-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-ping-api-openapi.yml
- filename: beazley-products-api-openapi.yml
  format: yaml
  label: Beazley Products API
  slug: beazley-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-products-api-openapi.yml
- filename: beazley-providers-api-openapi.yml
  format: yaml
  label: Beazley Providers API
  slug: beazley-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-providers-api-openapi.yml
- filename: beazley-rates-api-openapi.yml
  format: yaml
  label: Beazley Rates API
  slug: beazley-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-rates-api-openapi.yml
- filename: beazley-report-api-openapi.yml
  format: yaml
  label: Beazley Report API
  slug: beazley-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-report-api-openapi.yml
- filename: beazley-risks-api-openapi.yml
  format: yaml
  label: Beazley Risks API
  slug: beazley-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-risks-api-openapi.yml
- filename: beazley-search-api-openapi.yml
  format: yaml
  label: Beazley Search API
  slug: beazley-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-search-api-openapi.yml
- filename: beazley-faqs-api-openapi.yml
  format: yaml
  label: Beazley Faqs API
  slug: beazley-faqs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/openapi/beazley-faqs-api-openapi.yml
consequence_counts:
  read: 26
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Beazley Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 39
overview: 'Beazley exposes 39 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Beazley
provider_slug: beazley
slug: beazley-agentic-access
source_filename: beazley-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/beazley-audit-api-openapi.yml, openapi/beazley-check-api-openapi.yml, openapi/beazley-contacts-api-openapi.yml,\n  openapi/beazley-currencies-api-openapi.yml, openapi/beazley-cyber-api-openapi.yml, openapi/beazley-definitions-api-openapi.yml,\n  openapi/beazley-faqs-api-openapi.yml, openapi/beazley-health-api-openapi.yml, openapi/beazley-lockstate-api-openapi.yml,\n  openapi/beazley-microsites-api-openapi.yml, openapi/beazley-organisations-api-openapi.yml,\n  openapi/beazley-people-api-openapi.yml, openapi/beazley-ping-api-openapi.yml, openapi/beazley-products-api-openapi.yml,\n  openapi/beazley-providers-api-openapi.yml, openapi/beazley-rates-api-openapi.yml, openapi/beazley-report-api-openapi.yml,\n  openapi/beazley-risks-api-openapi.yml, openapi/beazley-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point\
  \ for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 13\n    connected: 26\n  by_consequence:\n    write: 13\n    read: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /audit/lookups\n  method: post\n  operationId: 5893134739845516588448cb\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audit\n  method: get\n  operationId: 5893134739845516588448cd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check\n  method: post\n  operationId: 5893134739845516588448c8\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/\n  method: post\n  operationId: 561e208f8097920ed881e636\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Contacts/{id}\n  method: put\n  operationId: 561e208f8097920ed881e637\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: get\n  operationId: 561e208f8097920ed881e638\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: get\n  operationId: 561e208f8097920ed881e639\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /currencies\n  method: get\n  operationId: 56d088f797fe1e081ca252ec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Cyber\n  method: post\n  operationId: 5804a8ff8097920fbc0ae7ea\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /definitions\n  method: get\n  operationId: 596757de398455123cd32ae7\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /definitions\n  method: post\n  operationId: 596872adc8b9bbc2a3352428\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /definitions/\n  method: get\n  operationId: 5971dd5476b7b3f0e01a426f\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faqs/\n  method: get\n  operationId: 59675bb966f3f16555c931b0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faqs\n  method: get\n  operationId: 5972212f109c6c8fce68fc40\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: post\n  operationId: 5893134739845516588448cc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lockstate/{id}\n  method: get\n  operationId: 554a0e3f8097920d90ff4e34\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lockstate/{id}\n  method: put\n  operationId: 554a108d8097920d90ff4e36\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /microsites/{id}/contacts\n  method: get\n  operationId: 561e208f8097920ed881e63a\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /microsites/\n  method: get\n  operationId: 561e208f8097920ed881e63c\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /microsites/{id}/organisations\n  method: get\n  operationId: 561e208f8097920ed881e640\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisations/{id}/contacts\n  method: get\n  operationId: 561e208f8097920ed881e63b\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /organisations/{id}\n  method: put\n  operationId: 561e208f8097920ed881e63d\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisations/{id}\n  method: get\n  operationId: 561e208f8097920ed881e63e\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisations\n  method: get\n  operationId: 561e208f8097920ed881e63f\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisations/{id}/organisations\n  method: post\n  operationId: 57236b6697fe1e136834c547\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people\n  method: get\n  operationId: 54e21d5297fe1e08786b4f2d\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{rid}\n  method: get\n  operationId: 54e21d5297fe1e08786b4f2e\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/profileimage\n  method: get\n  operationId: 54e21d5297fe1e08786b4f2f\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /People/deleted/\n  method: get\n  operationId: 5502bd2980979213687779a2\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/profileimagebyemail/\n  method: get\n  operationId: 5720682580979201c899e68d\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping/\n  method: get\n  operationId: 561e208f8097920ed881e641\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{term}\n  method: get\n  operationId: 59675c4259efa7b3b8c0fa3b\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers\n  method: get\n  operationId: 56d088f797fe1e081ca252eb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /rates\n  method: get\n  operationId: 56d088f797fe1e081ca252ea\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report\n  method: post\n  operationId: 5893134739845516588448ca\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risks/{id}\n  method: get\n  operationId: 5538d88d97fe1e0ff06f4248\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risks/{id}\n  method: put\n  operationId: 5538d88d97fe1e0ff06f424a\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risks/\n  method: post\n  operationId: 5538d88d97fe1e0ff06f4249\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: post\n  operationId: 5893134739845516588448c9\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beazley/refs/heads/main/agentic-access/beazley-agentic-access.yml
summary_line: 39 operations · 13 acting
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Cyber Insurance
- Specialty Insurance
- Lloyd's of London
- Underwriting
- Risk Data
- Brokers
- Carrier
---
