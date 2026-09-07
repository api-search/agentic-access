---
acting_count: 1
action_class_counts:
  acting: 1
api_specs:
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Projects and Plans API
  slug: dronedeploy-projects-and-plans-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Maps and Exports API
  slug: dronedeploy-maps-and-exports-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Annotations and Issues API
  slug: dronedeploy-annotations-and-issues-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Uploads and Images API
  slug: dronedeploy-uploads-and-images-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Users and Organizations API
  slug: dronedeploy-users-and-organizations-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Reports API
  slug: dronedeploy-reports-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Webhooks API
  slug: dronedeploy-webhooks-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
consequence_counts:
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dronedeploy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 1
overview: 'DroneDeploy exposes 1 API operation that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DroneDeploy
provider_slug: dronedeploy
slug: dronedeploy-agentic-access
source_filename: dronedeploy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/drone-deploy-graphql-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1\n  by_action_class:\n    acting: 1\n  by_consequence:\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /graphql\n  method: post\n  operationId: executeGraphQLOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/agentic-access/dronedeploy-agentic-access.yml
summary_line: 1 operation · 1 acting
tags:
- Drone Mapping
- Reality Capture
- Aerial Analytics
- Geospatial
- GraphQL
- Photogrammetry
---
