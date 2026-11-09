---
acting_count: 0
action_class_counts:
  connected: 19
api_specs:
- filename: aiwebsignals-com-agent-experience-api-openapi.yml
  format: yaml
  label: AIWebSignals Agent Experience API
  slug: aiwebsignals-com-agent-experience-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiwebsignals-com/openapi/aiwebsignals-com-agent-experience-api-openapi.yml
- filename: aiwebsignals-com-agent-reflective-api-openapi.yml
  format: yaml
  label: AIWebSignals Agent Reflective API
  slug: aiwebsignals-com-agent-reflective-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiwebsignals-com/openapi/aiwebsignals-com-agent-reflective-api-openapi.yml
- filename: aiwebsignals-com-discovery-api-openapi.yml
  format: yaml
  label: AIWebSignals Discovery API
  slug: aiwebsignals-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiwebsignals-com/openapi/aiwebsignals-com-discovery-api-openapi.yml
- filename: aiwebsignals-com-network-api-openapi.yml
  format: yaml
  label: AIWebSignals Network API
  slug: aiwebsignals-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiwebsignals-com/openapi/aiwebsignals-com-network-api-openapi.yml
- filename: aiwebsignals-com-readiness-api-openapi.yml
  format: yaml
  label: AIWebSignals Readiness API
  slug: aiwebsignals-com-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiwebsignals-com/openapi/aiwebsignals-com-readiness-api-openapi.yml
- filename: aiwebsignals-com-research-api-openapi.yml
  format: yaml
  label: AIWebSignals Research API
  slug: aiwebsignals-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiwebsignals-com/openapi/aiwebsignals-com-research-api-openapi.yml
- filename: aiwebsignals-com-self-observation-api-openapi.yml
  format: yaml
  label: AIWebSignals Self Observation API
  slug: aiwebsignals-com-self-observation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiwebsignals-com/openapi/aiwebsignals-com-self-observation-api-openapi.yml
- filename: aiwebsignals-com-well-known-api-openapi.yml
  format: yaml
  label: AIWebSignals .well Known API
  slug: aiwebsignals-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiwebsignals-com/openapi/aiwebsignals-com-well-known-api-openapi.yml
consequence_counts:
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aiwebsignals Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'AIWebSignals exposes 19 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AIWebSignals
provider_slug: aiwebsignals-com
slug: aiwebsignals-com-agentic-access
source_filename: aiwebsignals-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aiwebsignals-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 19\n  by_consequence:\n    read: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /.well-known/aiwebsignals.json\n  method: get\n  operationId: getMachineDiscoveryManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/capabilities\n  method: get\n  operationId: getMachineCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine-pricing\n\
  \  method: get\n  operationId: getMachinePricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/scan\n  method: get\n  operationId: scanAiWebReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report\n  method: get\n  operationId: getAiWebReadinessReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history\n  method: get\n  operationId: getAiWebReadinessHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/evaluate\n  method: get\n  operationId: evaluateAiWebReadinessOneCall\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/machine/connection-doctor\n  method: get\n  operationId: diagnoseMachineAgentConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/site-network.json\n  method: get\n  operationId: getRelatedSiteNetwork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/machine-native-experience.json\n  method: get\n  operationId: getMachineNativeExperienceFramework\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-experience-research.json\n  method: get\n  operationId: getAgentExperienceResearch\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-experience/question\n  method: get\n  operationId: getAgentExperienceQuestion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-reflective-research.json\n  method: get\n  operationId: getAgentReflectiveResearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-reflective/question\n  method: get\n  operationId: getAgentReflectiveQuestion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/research/interoperability-evidence\n  method: get\n  operationId: getInteroperabilityEvidence\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/self-observation\n  method: get\n  operationId: getSelfObservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/research/regulated-commerce\n  method: get\n  operationId: getRegulatedResearchLibrary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/research/regulated-commerce/{slug}\n  method: get\n  operationId: getRegulatedResearchArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/compare\n  method: get\n  operationId: comparePublicMachineWebEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aiwebsignals-com/agentic-access/aiwebsignals-com-agentic-access.yml
summary_line: 19 operations
tags:
- Artificial Intelligence
- Web
- Signals
- Analytics
- Machine Access
- CrawlerReadiness
---
