---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 30
api_specs:
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Organizations API
  slug: classy-org-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Campaigns API
  slug: classy-org-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Fundraising Pages API
  slug: classy-org-fundraising-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Fundraising Teams API
  slug: classy-org-fundraising-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Transactions API
  slug: classy-org-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Recurring Donation Plans API
  slug: classy-org-recurring-donation-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Members API
  slug: classy-org-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Supporters API
  slug: classy-org-supporters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
- filename: classy-org-openapi.yml
  format: yaml
  label: Classy Designations API
  slug: classy-org-designations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/openapi/classy-org-openapi.yml
consequence_counts:
  physical: 1
  read: 30
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Classy Org Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactions/{id}/acknowledgements
operation_count: 51
overview: 'Classy exposes 51 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 20 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Classy
provider_slug: classy-org
slug: classy-org-agentic-access
source_filename: classy-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/classy-org-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 51\n  by_action_class:\n    acting: 21\n    connected: 30\n  by_consequence:\n    write: 20\n    read: 30\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth2/auth\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/campaigns\n  method: get\n  operationId: listOrganizationCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/campaigns\n  method: post\n  operationId: createOrganizationCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/designations\n  method: get\n  operationId: listOrganizationDesignations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/designations\n\
  \  method: post\n  operationId: createOrganizationDesignation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/fundraising-pages\n  method: get\n  operationId: listOrganizationFundraisingPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/supporters\n  method: get\n  operationId: listOrganizationSupporters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/supporters\n  method: post\n  operationId: createOrganizationSupporter\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{id}/transactions\n  method: get\n  operationId: listOrganizationTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/recurring-donation-plans\n  method: get\n  operationId: listOrganizationRecurringDonationPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}/source-tracking-codes\n  method: get\n  operationId: listOrganizationSourceTrackingCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /campaigns/{id}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}\n  method: put\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/overview\n  method: get\n  operationId: getCampaignOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/publish\n  method: post\n  operationId: publishCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/unpublish\n  method: post\n  operationId: unpublishCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/deactivate\n  method: post\n  operationId: deactivateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/fundraising-pages\n  method: get\n  operationId: listCampaignFundraisingPages\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/fundraising-pages\n  method: post\n  operationId: createCampaignFundraisingPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/fundraising-teams\n  method: get\n  operationId: listCampaignFundraisingTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/fundraising-teams\n  method: post\n  operationId: createCampaignFundraisingTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/designations\n  method: get\n  operationId: listCampaignDesignations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/unassigned-designations\n  method: get\n  operationId: listCampaignUnassignedDesignations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/transactions\n  method: get\n  operationId: listCampaignTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/transactions\n  method: post\n  operationId: createCampaignTransaction\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/source-tracking-codes\n  method: get\n  operationId: listCampaignSourceTrackingCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fundraising-pages/{id}\n  method: get\n  operationId: getFundraisingPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fundraising-pages/{id}\n  method: put\n  operationId: updateFundraisingPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fundraising-pages/{id}\n  method: delete\n  operationId: deleteFundraisingPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fundraising-pages/{id}/overview\n  method: get\n  operationId: getFundraisingPageOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fundraising-teams/{id}\n  method: get\n  operationId: getFundraisingTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fundraising-teams/{id}\n  method: put\n  operationId: updateFundraisingTeam\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fundraising-teams/{id}\n  method: delete\n  operationId: deleteFundraisingTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fundraising-teams/{id}/overview\n  method: get\n  operationId: getFundraisingTeamOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fundraising-teams/{id}/fundraising-pages\n  method: post\n  operationId: createFundraisingTeamFundraisingPage\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{id}\n  method: put\n  operationId: updateTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/{id}/items\n  method: get\n  operationId: listTransactionItems\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{id}/acknowledgements\n  method: get\n  operationId: listTransactionAcknowledgements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{id}/acknowledgements\n  method: post\n  operationId: createTransactionAcknowledgement\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recurring-donation-plans/{id}\n  method: get\n  operationId: getRecurringDonationPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /recurring-donation-plans/{id}\n  method: put\n  operationId: updateRecurringDonationPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recurring-donation-plans/{id}/transactions\n  method: get\n  operationId: listRecurringDonationPlanTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members/{id}\n  method: get\n  operationId: getMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members/{id}/fundraising-pages\n  method: get\n  operationId: listMemberFundraisingPages\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members/{id}/recurring-donation-plans\n  method: get\n  operationId: listMemberRecurringDonationPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supporters/{id}\n  method: get\n  operationId: getSupporter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supporters/{id}\n  method: put\n  operationId: updateSupporter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designations/{id}\n  method: get\n  operationId: getDesignation\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /designations/{id}\n  method: put\n  operationId: updateDesignation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/classy-org/refs/heads/main/agentic-access/classy-org-agentic-access.yml
summary_line: 51 operations · 21 acting
tags:
- Nonprofit
- Fundraising
- Donations
- Peer to Peer
- Philanthropy
- Payments
- GoFundMe Pro
---
