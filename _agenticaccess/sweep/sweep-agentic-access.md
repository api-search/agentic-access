---
acting_count: 358
action_class_counts:
  acting: 358
  connected: 340
api_specs:
- filename: sweep-api-openapi.yml
  format: yaml
  label: Sweep API
  slug: sweep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sweep/refs/heads/main/openapi/sweep-api-openapi.yml
consequence_counts:
  read: 340
  safety-critical: 358
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 358
kind: agentic-access
layout: agentic-access
method: generated
name: Sweep Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /account-selection/accounts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account-selection/accounts/{accountId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /agentic-features
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /agentic-features/data-access-settings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai-agents
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /ai-agents/artifacts/{id}/public
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /ai-agents/artifacts/{id}/share
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /ai-agents/chats/{chatId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /ai-agents/chats/{chatId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /ai-agents/chats/{chatId}/favorite
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai-agents/chats/{chatId}/feedback/{runId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /ai-agents/chats/{chatId}/messages/{messageIndex}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /ai-agents/chats/{chatId}/name
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /ai-agents/monitoring/{agentId}/issues/{issueId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai-agents/process-mining/{funnelMapId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /ai-agents/stream/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /ai-agents/{agentId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai-agents/{agentId}/best-practices
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /ai-agents/{agentId}/best-practices
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai-agents/{agentId}/chats
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai-agents/{agentId}/chats/{chatId}/add-to-agent
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /ai-agents/{agentId}/chats/{chatId}/folder
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai-agents/{agentId}/chats/{chatId}/mcp-tool-approval
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /ai-agents/{agentId}/configurations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ai-agents/{agentId}/files/confirm-upload
operation_count: 698
overview: 'Sweep exposes 698 API operations that an AI agent could call, of which 358 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 340 read and 358 safety-critical.


  358 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sweep
provider_slug: sweep
slug: sweep-agentic-access
source_filename: sweep-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/sweep-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 698\n  by_action_class:\n    connected: 340\n    acting: 358\n  by_consequence:\n    read: 340\n    safety-critical: 358\n  human_in_the_loop_required: 358\noperations:\n- path: /health\n  method: get\n  operationId: HealthController_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snowflake-orgs\n  method: post\n  operationId: SnowflakeOrgController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /snowflake-orgs/databases\n  method: post\n  operationId: SnowflakeOrgController_listDatabasesWithCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /snowflake-orgs/{orgId}\n  method: delete\n  operationId: SnowflakeOrgController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /servicenow-orgs\n  method: post\n  operationId: ServiceNowOrgController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /servicenow-orgs/{orgId}\n  method: patch\n  operationId: ServiceNowOrgController_reconnect\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /servicenow-orgs/{orgId}\n  method: delete\n  operationId: ServiceNowOrgController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /servicenow-orgs/{orgId}/fetch\n  method: post\n  operationId: ServiceNowOrgController_triggerFetch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /workato-orgs\n  method: post\n  operationId: WorkatoOrgController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n  \
  \    human-in-the-loop: required\n    audit: required\n- path: /documentation-platform/snowflake/search\n  method: get\n  operationId: DocumentationPlatformController_searchElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/snowflake/search-by-metadata\n  method: get\n  operationId: DocumentationPlatformController_findElementByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/snowflake/{metadataId}/dependencies\n  method: get\n  operationId: DocumentationPlatformController_getElementDependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/snowflake/{metadataId}/dependents\n  method: get\n\
  \  operationId: DocumentationPlatformController_getElementDependents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/snowflake/{metadataId}/summary\n  method: get\n  operationId: DocumentationPlatformController_getElementSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/snowflake/{metadataId}/source\n  method: get\n  operationId: DocumentationPlatformController_getElementSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/snowflake/{metadataId}/chat\n  method: post\n  operationId: DocumentationPlatformController_chatWithElement\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /documentation-platform/snowflake/{elementType}\n  method: get\n  operationId: DocumentationPlatformController_listElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/data360/search\n  method: get\n  operationId: DocumentationPlatformController_searchData360Elements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/data360/search-by-metadata\n  method: get\n  operationId: DocumentationPlatformController_findData360ElementByName\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/data360/{metadataId}/dependencies\n  method: get\n  operationId: DocumentationPlatformController_getData360ElementDependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/data360/{metadataId}/dependents\n  method: get\n  operationId: DocumentationPlatformController_getData360ElementDependents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/data360/{metadataId}/children\n  method: get\n  operationId: DocumentationPlatformController_getData360ElementChildren\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /documentation-platform/data360/{metadataId}/summary\n  method: get\n  operationId: DocumentationPlatformController_getData360ElementSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/data360/{metadataId}/source\n  method: get\n  operationId: DocumentationPlatformController_getData360ElementSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/data360/{metadataId}/chat\n  method: post\n  operationId: DocumentationPlatformController_chatWithData360Element\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n     \
  \ human-in-the-loop: required\n    audit: required\n- path: /documentation-platform/data360/{elementType}\n  method: get\n  operationId: DocumentationPlatformController_listData360Elements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/workato/search\n  method: get\n  operationId: DocumentationPlatformController_searchWorkatoElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/workato/search-by-metadata\n  method: get\n  operationId: DocumentationPlatformController_findWorkatoElementByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/workato/{metadataId}/dependencies\n  method: get\n  operationId:\
  \ DocumentationPlatformController_getWorkatoElementDependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/workato/{metadataId}/dependents\n  method: get\n  operationId: DocumentationPlatformController_getWorkatoElementDependents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/workato/{metadataId}/children\n  method: get\n  operationId: DocumentationPlatformController_getWorkatoElementChildren\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/workato/{metadataId}/source\n  method: get\n  operationId: DocumentationPlatformController_getWorkatoElementSource\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/workato/{metadataId}/summary\n  method: get\n  operationId: DocumentationPlatformController_getWorkatoElementSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/workato/{elementType}\n  method: get\n  operationId: DocumentationPlatformController_listWorkatoElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/hubspot/search\n  method: get\n  operationId: DocumentationPlatformController_searchHubspotElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/hubspot/search-by-metadata\n\
  \  method: get\n  operationId: DocumentationPlatformController_findHubspotElementByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/hubspot/{metadataId}/dependencies\n  method: get\n  operationId: DocumentationPlatformController_getHubspotElementDependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/hubspot/{metadataId}/dependents\n  method: get\n  operationId: DocumentationPlatformController_getHubspotElementDependents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/hubspot/{metadataId}/children\n  method: get\n  operationId: DocumentationPlatformController_getHubspotElementChildren\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/hubspot/{metadataId}/summary\n  method: get\n  operationId: DocumentationPlatformController_getHubspotElementSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/hubspot/{metadataId}/source\n  method: get\n  operationId: DocumentationPlatformController_getHubspotElementSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/hubspot/{metadataId}/chat\n  method: post\n  operationId: DocumentationPlatformController_chatWithHubspotElement\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /documentation-platform/hubspot/{elementType}\n  method: get\n  operationId: DocumentationPlatformController_listHubspotElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/servicenow/search\n  method: get\n  operationId: DocumentationPlatformController_searchServiceNowElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/servicenow/search-by-metadata\n  method: get\n  operationId: DocumentationPlatformController_findServiceNowElementByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/servicenow/tables/{tableName}/fields\n  method: get\n  operationId: DocumentationPlatformController_getServiceNowTableFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/servicenow/{metadataId}/summary\n  method: get\n  operationId: DocumentationPlatformController_getServiceNowElementSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/servicenow/{metadataId}/chat\n  method: post\n  operationId: DocumentationPlatformController_chatWithServiceNowElement\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /documentation-platform/servicenow/{metadataId}/source\n  method: get\n  operationId: DocumentationPlatformController_getServiceNowElementSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/servicenow/{metadataId}/choices\n  method: get\n  operationId: DocumentationPlatformController_getServiceNowFieldChoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/servicenow/{elementType}\n  method: get\n  operationId: DocumentationPlatformController_listServiceNowElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /documentation-platform/salesforce/objects\n  method: get\n  operationId: DocumentationPlatformController_listSalesforceObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/salesforce/element-types\n  method: get\n  operationId: DocumentationPlatformController_listSalesforceElementTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/salesforce/objects/{objectName}/elements\n  method: get\n  operationId: DocumentationPlatformController_getSalesforceObjectDetailElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/salesforce/objects/{objectName}/counters\n  method: get\n  operationId: DocumentationPlatformController_getSalesforceObjectCounters\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/salesforce/{elementType}\n  method: get\n  operationId: DocumentationPlatformController_listSalesforceElements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/salesforce/{metadataId}/dependencies\n  method: get\n  operationId: DocumentationPlatformController_getSalesforceElementDependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documentation-platform/salesforce/{metadataId}/dependents\n  method: get\n  operationId: DocumentationPlatformController_getSalesforceElementDependents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /homepage\n  method: get\n  operationId: HomepageController_loadHomepageStuff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webapp/config/opportunity-stage-options\n  method: get\n  operationId: WebappController_getOpportunityStageOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs\n  method: get\n  operationId: CrmOrgsController_getOrgs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/new\n  method: post\n  operationId: CrmOrgsController_createOrgs\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /crm-orgs/org/{orgId}/salesforce-oauth\n  method: get\n  operationId: CrmOrgsController_getSFDCOAuthPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}\n  method: get\n  operationId: CrmOrgsController_getOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}\n  method: patch\n  operationId: CrmOrgsController_updateOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /crm-orgs/org/{orgId}/emailTemplates\n  method: get\n  operationId: CrmOrgsController_getEmailTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}/object-types/{objectName}/child-relationship-names\n  method: get\n  operationId: CrmOrgsController_getChildRelationshipNames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}/apex-classes\n  method: get\n  operationId: CrmOrgsController_getApexClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/salesforce-oauth2-code\n  method: post\n  operationId: CrmOrgsController_handleSFDCOAuthAuthorizationCode\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /crm-orgs/org/{orgId}/connect-anyway\n  method: post\n  operationId: CrmOrgsController_connectAnyway\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /crm-orgs/org/{orgId}/object-types\n  method: get\n  operationId: CrmOrgsController_getObjectTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /crm-orgs/org/{orgId}/object-types-2\n  method: get\n  operationId: CrmOrgsController_getObjectTypes2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}/users/member-properties\n  method: get\n  operationId: CrmOrgsController_listUsersWithMemberProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}/users\n  method: get\n  operationId: CrmOrgsController_listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}/users/{userId}/timeOff\n  method: post\n  operationId: CrmOrgsController_createUserTimeOff\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /crm-orgs/org/{orgId}/users/{userId}/timeOff/{timeOffId}\n  method: put\n  operationId: CrmOrgsController_updateUserTimeOff\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /crm-orgs/org/{orgId}/users/{userId}/timeOff/{timeOffId}\n  method: delete\n  operationId: CrmOrgsController_deleteUserTimeOff\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /crm-orgs/org/{orgId}/queues\n  method: get\n  operationId: CrmOrgsController_listQueues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}/funnels-and-record-types\n  method: get\n  operationId: CrmOrgsController_getAllFunnelsAndRecordTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}/objects\n  method: get\n  operationId: CrmOrgsController_getSalesforceObjectTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}/objects/{objectName}/funnels-and-record-types\n  method: get\n  operationId: CrmOrgsController_getObjectFunnelsAndRecordTypes\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}/objects/{objectName}/record-types/{recordTypeName}\n  method: get\n  operationId: CrmOrgsController_getLeadingFieldCandidatesForRecordType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crm-orgs/org/{orgId}/sweep-permission-set-group-assignment\n  method: post\n  operationId: CrmOrgsController_assignPermissionSetGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /orgs\n  method: get\n  operationId: OrgsController_getAllOrgs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}\n  method: delete\n  operationId: OrgsController_deleteOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /orgs/{orgId}\n  method: get\n  operationId: OrgsController_getOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}\n  method: patch\n  operationId: OrgsController_renameOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /orgs/{orgId}/fetch\n  method: post\n  operationId: OrgsController_fetchWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /assignment_groups\n  method: get\n  operationId: AssignmentGroupsController_getAssignmentGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assignment_groups\n  method: post\n  operationId: AssignmentGroupsController_insertGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /assignment_groups/credit-queue\n  method: get\n  operationId: AssignmentGroupsController_getCreditQueue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assignment_groups/credit-queue\n  method: post\n  operationId: AssignmentGroupsController_createCreditQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /assignment_groups/credit-queue\n  method: put\n  operationId: AssignmentGroupsController_updateCreditQueue\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /assignment_groups/{groupId}\n  method: get\n  operationId: AssignmentGroupsController_getAssignmentGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assignment_groups/{groupId}\n  method: delete\n  operationId: AssignmentGroupsController_deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /assignment_groups/{groupId}\n  method: put\n  operationId: AssignmentGroupsController_updateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /funnels/funnel-name-availability\n  method: get\n  operationId: FunnelsController_checkFunnelNameAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funnels\n  method: post\n  operationId: FunnelsController_createFunnel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /funnels/convert-record-type\n  method: post\n  operationId: FunnelsController_convertRecordTypeToFunnel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /funnels/funnel-from-record-type\n  method: get\n  operationId: FunnelsController_getFunnelAndSnapshotIdFromRecordType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funnels/{funnelId}/snapshots\n  method: get\n  operationId: FunnelsController_getFunnelSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /funnels/{funnelId}/snapshots\n  method: post\n  operationId: FunnelsController_createFunnelSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /funnels/{funnelId}/snapshots/{snapshotId}\n  method: get\n  operationId: FunnelsController_getFunnelSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funnels/{funnelId}/snapshots/{snapshotId}\n  method: patch\n\n\n# --- truncated at 32 KB (232 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/sweep/refs/heads/main/agentic-access/sweep-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sweep/refs/heads/main/agentic-access/sweep-agentic-access.yml
summary_line: 698 operations · 358 acting · 358 human-in-the-loop
tags:
- Company
- Cloud
- Salesforce
- RevOps
- Metadata
- Governance
- AI Agents
- Model Context Protocol
- Automation
- Documentation
- API
- REST API
- OpenAPI
- Enterprise Systems
- Snowflake
- ServiceNow
- Data Governance
---
