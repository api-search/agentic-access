---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 12
api_specs:
- filename: microsoft-playwright-accountquotas-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Account Quotas API
  slug: microsoft-playwright-accountquotas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-accountquotas-api-openapi.yml
- filename: microsoft-playwright-accounts-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Accounts API
  slug: microsoft-playwright-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-accounts-api-openapi.yml
- filename: microsoft-playwright-operations-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Operations API
  slug: microsoft-playwright-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-operations-api-openapi.yml
- filename: microsoft-playwright-quotas-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Quotas API
  slug: microsoft-playwright-quotas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-quotas-api-openapi.yml
consequence_counts:
  read: 12
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Playwright Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Microsoft Playwright exposes 18 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Playwright
provider_slug: microsoft-playwright
slug: microsoft-playwright-agentic-access
source_filename: microsoft-playwright-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/microsoft-playwright-authmanager-openapi.yml, openapi/microsoft-playwright-management-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 12\n    acting: 6\n  by_consequence:\n    read: 12\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/{accountId}\n  method: get\n  operationId: Accounts_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://playwright.microsoft.com/.default\n- path: /accounts/{accountId}/access-tokens\n  method: get\n  operationId: AccessTokens_List\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://playwright.microsoft.com/.default\n- path: /accounts/{accountId}/access-tokens/{accessTokenId}\n  method: get\n  operationId: AccessTokens_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://playwright.microsoft.com/.default\n- path: /accounts/{accountId}/access-tokens/{accessTokenId}\n  method: put\n  operationId: AccessTokens_CreateOrReplace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://playwright.microsoft.com/.default\n- path: /accounts/{accountId}/access-tokens/{accessTokenId}\n\
  \  method: delete\n  operationId: AccessTokens_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://playwright.microsoft.com/.default\n- path: /accounts/{accountId}/browsers\n  method: get\n  operationId: Accounts_GetBrowsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://playwright.microsoft.com/.default\n- path: /providers/Microsoft.AzurePlaywrightService/operations\n  method: get\n  operationId: Operations_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/providers/Microsoft.AzurePlaywrightService/accounts\n\
  \  method: get\n  operationId: Accounts_ListBySubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/providers/Microsoft.AzurePlaywrightService/checkNameAvailability\n  method: post\n  operationId: Accounts_CheckNameAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/providers/Microsoft.AzurePlaywrightService/locations/{location}/quotas\n  method: get\n  operationId: Quotas_ListBySubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/providers/Microsoft.AzurePlaywrightService/locations/{location}/quotas/{quotaName}\n  method: get\n  operationId: Quotas_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.AzurePlaywrightService/accounts\n  method: get\n  operationId: Accounts_ListByResourceGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.AzurePlaywrightService/accounts/{accountName}\n  method: get\n  operationId: Accounts_Get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.AzurePlaywrightService/accounts/{accountName}\n  method: put\n  operationId: Accounts_CreateOrUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.AzurePlaywrightService/accounts/{accountName}\n  method: patch\n  operationId: Accounts_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.AzurePlaywrightService/accounts/{accountName}\n  method: delete\n  operationId: Accounts_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.AzurePlaywrightService/accounts/{accountName}/quotas\n  method: get\n  operationId: AccountQuotas_ListByAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n- path: /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.AzurePlaywrightService/accounts/{accountName}/quotas/{quotaName}\n  method: get\n  operationId: AccountQuotas_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - user_impersonation\n"
source_yaml_url: https://artifacts.apis.io/microsoft-playwright/agentic-access/microsoft-playwright-agentic-access.yml
summary_line: 18 operations · 6 acting
tags:
- Browser Automation
- End-to-End Testing
- Microsoft
- Testing
- Open Source
- MCP
- Microsoft Azure
---
