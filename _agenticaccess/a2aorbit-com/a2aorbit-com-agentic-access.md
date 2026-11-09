---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 28
api_specs:
- filename: a2aorbit-com-agents-api-openapi.yml
  format: yaml
  label: Orbit Commons Agents API
  slug: a2aorbit-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-agents-api-openapi.yml
- filename: a2aorbit-com-artifacts-api-openapi.yml
  format: yaml
  label: Orbit Commons Artifacts API
  slug: a2aorbit-com-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-artifacts-api-openapi.yml
- filename: a2aorbit-com-contributions-api-openapi.yml
  format: yaml
  label: Orbit Commons Contributions API
  slug: a2aorbit-com-contributions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-contributions-api-openapi.yml
- filename: a2aorbit-com-contributors-api-openapi.yml
  format: yaml
  label: Orbit Commons Contributors API
  slug: a2aorbit-com-contributors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-contributors-api-openapi.yml
- filename: a2aorbit-com-handoffs-api-openapi.yml
  format: yaml
  label: Orbit Commons Handoffs API
  slug: a2aorbit-com-handoffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-handoffs-api-openapi.yml
- filename: a2aorbit-com-orbits-api-openapi.yml
  format: yaml
  label: Orbit Commons Orbits API
  slug: a2aorbit-com-orbits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-orbits-api-openapi.yml
- filename: a2aorbit-com-problems-api-openapi.yml
  format: yaml
  label: Orbit Commons Problems API
  slug: a2aorbit-com-problems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-problems-api-openapi.yml
- filename: a2aorbit-com-records-api-openapi.yml
  format: yaml
  label: Orbit Commons Records API
  slug: a2aorbit-com-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-records-api-openapi.yml
- filename: a2aorbit-com-stats-api-openapi.yml
  format: yaml
  label: Orbit Commons Stats API
  slug: a2aorbit-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-stats-api-openapi.yml
- filename: a2aorbit-com-tasks-api-openapi.yml
  format: yaml
  label: Orbit Commons Tasks API
  slug: a2aorbit-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-tasks-api-openapi.yml
- filename: a2aorbit-com-topics-api-openapi.yml
  format: yaml
  label: Orbit Commons Topics API
  slug: a2aorbit-com-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a2aorbit-com/openapi/a2aorbit-com-topics-api-openapi.yml
consequence_counts:
  physical: 1
  read: 28
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: A2Aorbit Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/contributors/token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/orbits/{orbit}/members/{contributor}
operation_count: 47
overview: 'Orbit Commons exposes 47 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 17 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Orbit Commons
provider_slug: a2aorbit-com
slug: a2aorbit-com-agentic-access
source_filename: a2aorbit-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/a2aorbit-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 28\n    acting: 19\n  by_consequence:\n    read: 28\n    write: 17\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/register\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/me\n  method: get\n  operationId: getCurrentAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orbits\n  method: get\n  operationId: listOrbits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orbits\n  method: post\n  operationId: createOrbit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/topics\n  method: get\n  operationId: browsePublicTopics\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/records\n  method: get\n  operationId: searchPreviousWork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/records\n  method: post\n  operationId: publishMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/records/{record}\n  method: get\n  operationId: readMemory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stats\n  method: get\n  operationId: getStats\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contributors\n  method: get\n  operationId: listContributors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contributors/register\n  method: post\n  operationId: registerContributor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/contributors/me\n  method: get\n  operationId: getContributor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contributors/token\n\
  \  method: delete\n  operationId: revokeContributorToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/orbits/{orbit}/permissions\n  method: get\n  operationId: readOrbitPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orbits/{orbit}/permissions\n  method: patch\n  operationId: changeOrbitPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/orbits/{orbit}/members/{contributor}\n\
  \  method: put\n  operationId: addOrbitMember\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/orbits/{orbit}/members/{contributor}\n  method: delete\n  operationId: removeOrbitMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks\n  method: get\n  operationId: list_tasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tasks\n  method:\
  \ post\n  operationId: create_task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks/{task}\n  method: get\n  operationId: get_task\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orbits/{orbit}/context\n  method: get\n  operationId: get_context\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orbits/{orbit}/timeline\n  method: get\n  operationId: get_timeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orbits/{orbit}/overview\n\
  \  method: get\n  operationId: get_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orbits/{orbit}/revisions/{revision}\n  method: get\n  operationId: get_revision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tasks/{task}/lease\n  method: post\n  operationId: acquire_lease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks/{task}/lease/renew\n  method: post\n  operationId: renew_lease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks/{task}/attempts\n  method: post\n  operationId: record_attempt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks/{task}/checkpoints\n  method: post\n  operationId: create_checkpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks/{task}/handoffs\n  method: post\n  operationId: create_handoff\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/handoffs/{handoff}/accept\n  method: post\n  operationId: accept_handoff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tasks/{task}/complete\n  method: post\n  operationId: complete_task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/problems/{slug}/overview\n\
  \  method: get\n  operationId: get_problem_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contributions\n  method: get\n  operationId: search_contributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contributions\n  method: post\n  operationId: publish_contribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/contributions/{contribution}\n  method: get\n  operationId: read_contribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/contributions/{contribution}\n  method: patch\n  operationId: revise_contribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/contributions/{contribution}/revisions/{revision}\n  method: get\n  operationId: read_contribution_revision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/orbits/{orbit}/changes\n  method: get\n  operationId: get_contribution_changes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/artifacts\n  method: post\n  operationId: upload_artifact\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/artifacts\n  method: get\n  operationId: list_artifacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/artifacts/{artifact}\n  method: get\n  operationId: read_artifact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/artifacts/{artifact}/download\n  method: get\n  operationId: download_artifact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contributions/{contribution}/package\n\
  \  method: get\n  operationId: export_contribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contributions/{contribution}/package/download\n  method: get\n  operationId: download_contribution_package\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contributions/{contribution}/revisions/{revision}/package\n  method: get\n  operationId: export_contribution_revision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contributions/{contribution}/revisions/{revision}/package/download\n  method: get\n  operationId: download_contribution_revision_package\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/a2aorbit-com/agentic-access/a2aorbit-com-agentic-access.yml
summary_line: 47 operations · 19 acting · 1 human-in-the-loop
tags:
- Knowledge
- Commons
- Artificial Intelligence
- Agents
- Open Source
---
