---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 7
api_specs:
- filename: salesforce-knowledge-management-rest-api-openapi.yml
  format: yaml
  label: Salesforce Knowledge REST API
  slug: salesforce-knowledge-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-knowledge-management/refs/heads/main/openapi/salesforce-knowledge-management-rest-api-openapi.yml
consequence_counts:
  read: 7
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Salesforce Knowledge Management Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Salesforce Knowledge Management exposes 11 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Salesforce Knowledge Management
provider_slug: salesforce-knowledge-management
slug: salesforce-knowledge-management-agentic-access
source_filename: salesforce-knowledge-management-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/salesforce-knowledge-management-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 7\n    acting: 4\n  by_consequence:\n    read: 7\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /sobjects/KnowledgeArticle\n  method: get\n  operationId: listKnowledgeArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sobjects/KnowledgeArticle/{articleId}\n  method: get\n  operationId: getKnowledgeArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /support/knowledgeArticles\n  method: get\n  operationId: searchKnowledgeArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /support/knowledgeArticles/{articleId}\n  method: get\n  operationId: getKnowledgeArticleDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sobjects/KnowledgeArticleVersion\n  method: post\n  operationId: createKnowledgeArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sobjects/KnowledgeArticleVersion/{versionId}\n  method: patch\n  operationId: updateKnowledgeArticle\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sobjects/KnowledgeArticleVersion/{versionId}\n  method: delete\n  operationId: deleteKnowledgeArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/standard/publishKnowledgeArticles\n  method: post\n  operationId: publishKnowledgeArticles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /support/dataCategoryGroups\n  method: get\n  operationId: listDataCategoryGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /support/dataCategoryGroups/{group}/dataCategories\n  method: get\n  operationId: listDataCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /support/suggestedArticles\n  method: get\n  operationId: getSuggestedArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-knowledge-management/refs/heads/main/agentic-access/salesforce-knowledge-management-agentic-access.yml
summary_line: 11 operations · 4 acting
tags:
- Articles
- CRM
- Customer Service
- Documentation
- Knowledge Management
- Support
---
