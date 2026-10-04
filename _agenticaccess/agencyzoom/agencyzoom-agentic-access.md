---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 19
api_specs:
- filename: agencyzoom-authentication-api-openapi.yml
  format: yaml
  label: AgencyZoom Authentication API
  slug: agencyzoom-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-authentication-api-openapi.yml
- filename: agencyzoom-configuration-api-openapi.yml
  format: yaml
  label: AgencyZoom Configuration API
  slug: agencyzoom-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-configuration-api-openapi.yml
- filename: agencyzoom-customers-api-openapi.yml
  format: yaml
  label: AgencyZoom Customers API
  slug: agencyzoom-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-customers-api-openapi.yml
- filename: agencyzoom-email-api-openapi.yml
  format: yaml
  label: AgencyZoom Email API
  slug: agencyzoom-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-email-api-openapi.yml
- filename: agencyzoom-leads-api-openapi.yml
  format: yaml
  label: AgencyZoom Leads API
  slug: agencyzoom-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-leads-api-openapi.yml
- filename: agencyzoom-opportunities-api-openapi.yml
  format: yaml
  label: AgencyZoom Opportunities API
  slug: agencyzoom-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-opportunities-api-openapi.yml
- filename: agencyzoom-pipelines-api-openapi.yml
  format: yaml
  label: AgencyZoom Pipelines API
  slug: agencyzoom-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-pipelines-api-openapi.yml
- filename: agencyzoom-policies-api-openapi.yml
  format: yaml
  label: AgencyZoom Policies API
  slug: agencyzoom-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/openapi/agencyzoom-policies-api-openapi.yml
consequence_counts:
  read: 19
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agencyzoom Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 36
overview: 'AgencyZoom exposes 36 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgencyZoom
provider_slug: agencyzoom
slug: agencyzoom-agentic-access
source_filename: agencyzoom-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/agencyzoom-authentication-api-openapi.yml, openapi/agencyzoom-configuration-api-openapi.yml,\n  openapi/agencyzoom-customers-api-openapi.yml, openapi/agencyzoom-email-api-openapi.yml, openapi/agencyzoom-leads-api-openapi.yml,\n  openapi/agencyzoom-opportunities-api-openapi.yml, openapi/agencyzoom-pipelines-api-openapi.yml,\n  openapi/agencyzoom-policies-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 17\n    connected: 19\n  by_consequence:\n    write: 17\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/api/auth/login\n  method: post\n  operationId: postV1ApiAuthLogin\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/auth/ssologin\n  method: post\n  operationId: postV1ApiAuthSsologin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/auth/logout\n  method: post\n  operationId: postV1ApiAuthLogout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/product-categories\n  method:\
  \ get\n  operationId: getV1ApiProductCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/product-lines\n  method: get\n  operationId: getV1ApiProductLines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/employees\n  method: get\n  operationId: getV1ApiEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/carriers\n  method: get\n  operationId: getV1ApiCarriers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/custom-fields\n  method: get\n  operationId: getV1ApiCustomFields\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/customers\n  method: post\n  operationId: postV1ApiCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/customers/{customerId}\n  method: get\n  operationId: getV1ApiCustomersByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/customers/{customerId}\n  method: put\n  operationId: putV1ApiCustomersByCustomerId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/customers/{customerId}\n  method: delete\n\
  \  operationId: deleteV1ApiCustomersByCustomerId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/customers/{customerId}/policies\n  method: get\n  operationId: getV1ApiCustomersByCustomerIdPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/customers/{customerId}/ams-policies\n  method: get\n  operationId: getV1ApiCustomersByCustomerIdAmsPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/email-thread/list\n  method: post\n  operationId: postV1ApiEmailThreadList\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/email-thread/email-thread-detail\n  method: post\n  operationId: postV1ApiEmailThreadEmailThreadDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/leads/list\n  method: post\n  operationId: postV1ApiLeadsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/leads/create\n  method: post\n  operationId: postV1ApiLeadsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/leads/create-biz-lead\n  method: post\n\
  \  operationId: postV1ApiLeadsCreateBizLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/leads/{leadId}\n  method: get\n  operationId: getV1ApiLeadsByLeadId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/leads/{leadId}\n  method: put\n  operationId: putV1ApiLeadsByLeadId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/leads/{leadId}/sold\n  method: post\n  operationId: postV1ApiLeadsByLeadIdSold\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/leads/{leadId}/opportunities\n  method: get\n  operationId: getV1ApiLeadsByLeadIdOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/leads/{leadId}/quotes\n  method: get\n  operationId: getV1ApiLeadsByLeadIdQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/leads/{leadId}/notes\n  method: get\n  operationId: getV1ApiLeadsByLeadIdNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/api/leads/{leadId}/notes\n  method: post\n  operationId: postV1ApiLeadsByLeadIdNotes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/opportunities\n  method: post\n  operationId: postV1ApiOpportunities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/opportunities/{opportunityId}\n  method: get\n  operationId: getV1ApiOpportunitiesByOpportunityId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/api/opportunities/{opportunityId}\n  method: put\n  operationId: putV1ApiOpportunitiesByOpportunityId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/opportunities/{opportunityId}/driver\n  method: post\n  operationId: postV1ApiOpportunitiesByOpportunityIdDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/opportunities/{opportunityId}/vehicle\n  method: post\n  operationId: postV1ApiOpportunitiesByOpportunityIdVehicle\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/pipelines\n  method: get\n  operationId: getV1ApiPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/pipelines-and-stages\n  method: get\n  operationId: getV1ApiPipelinesAndStages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api/policies/create\n  method: post\n  operationId: postV1ApiPoliciesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/policies/{policyId}\n  method: put\n  operationId: putV1ApiPoliciesByPolicyId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api/policies/update-tags\n  method: post\n  operationId: postV1ApiPoliciesUpdateTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agencyzoom/refs/heads/main/agentic-access/agencyzoom-agentic-access.yml
summary_line: 36 operations · 17 acting
tags:
- Insurance
- Insurtech
- CRM
- Sales Automation
- Agency Management
- Customer Retention
---
