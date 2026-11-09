---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 18
api_specs:
- filename: animalchecklist-com-account-api-openapi.yml
  format: yaml
  label: animalchecklist-com Account API
  slug: animalchecklist-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-account-api-openapi.yml
- filename: animalchecklist-com-catalogue-api-openapi.yml
  format: yaml
  label: animalchecklist-com Catalogue API
  slug: animalchecklist-com-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-catalogue-api-openapi.yml
- filename: animalchecklist-com-diagnostics-api-openapi.yml
  format: yaml
  label: animalchecklist-com Diagnostics API
  slug: animalchecklist-com-diagnostics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-diagnostics-api-openapi.yml
- filename: animalchecklist-com-leaderboard-api-openapi.yml
  format: yaml
  label: animalchecklist-com Leaderboard API
  slug: animalchecklist-com-leaderboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-leaderboard-api-openapi.yml
- filename: animalchecklist-com-quiz-api-openapi.yml
  format: yaml
  label: animalchecklist-com Quiz API
  slug: animalchecklist-com-quiz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-quiz-api-openapi.yml
- filename: animalchecklist-com-recognition-api-openapi.yml
  format: yaml
  label: animalchecklist-com Recognition API
  slug: animalchecklist-com-recognition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-recognition-api-openapi.yml
- filename: animalchecklist-com-sightings-api-openapi.yml
  format: yaml
  label: animalchecklist-com Sightings API
  slug: animalchecklist-com-sightings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-sightings-api-openapi.yml
consequence_counts:
  read: 18
  safety-critical: 1
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Animalchecklist Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /auth/mcp-tokens/{id}
operation_count: 41
overview: 'animalchecklist-com exposes 41 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 22 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: animalchecklist-com
provider_slug: animalchecklist-com
slug: animalchecklist-com-agentic-access
source_filename: animalchecklist-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/animalchecklist-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    connected: 18\n    acting: 23\n  by_consequence:\n    read: 18\n    write: 22\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /taxa\n  method: get\n  operationId: getReferenceTaxa\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /taxa/{inatId}\n  method: get\n  operationId: getInatTaxon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /breeds\n\
  \  method: get\n  operationId: getBreedDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leaderboard\n  method: get\n  operationId: getLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quiz/rounds\n  method: post\n  operationId: createQuizRound\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quiz/rounds/{id}\n  method: get\n  operationId: getQuizRound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quiz/rounds/{id}\n\
  \  method: delete\n  operationId: deleteGuestQuizRound\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quiz/rounds/{id}/answers\n  method: post\n  operationId: answerQuizRound\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quiz/rounds/{id}/claim\n  method: post\n  operationId: claimQuizRound\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /quiz/rounds/{id}/photos/{index}\n  method: get\n  operationId: getQuizPhoto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quiz/score\n  method: get\n  operationId: getQuizScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/magic-link/request\n  method: post\n  operationId: requestMagicLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/magic-link/consume\n  method: post\n  operationId: consumeMagicLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/logout\n  method: post\n  operationId: logoutAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/passkeys/registration/options\n  method: post\n  operationId: passkeyRegistrationOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/passkeys/registration/verify\n  method: post\n  operationId:\
  \ verifyPasskeyRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/passkeys/authentication/options\n  method: post\n  operationId: passkeyAuthenticationOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/passkeys/authentication/verify\n  method: post\n  operationId: verifyPasskeyAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/passkeys\n  method: get\n  operationId: listPasskeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/passkeys/{id}\n  method: delete\n  operationId: deletePasskey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/mcp-tokens\n  method: get\n  operationId: listMcpTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/mcp-tokens\n  method: post\n  operationId: createMcpToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/mcp-tokens/{id}\n  method: delete\n  operationId: revokeMcpToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: delete\n  operationId: deleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/import\n  method: post\n  operationId: importAnonymousSightings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/export\n  method: get\n  operationId: exportAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /animals\n  method: post\n  operationId: searchUnseenAnimals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /animals\n  method: get\n  operationId: searchAnimals\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /animals/{id}\n  method: get\n  operationId: getAnimal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recognitions\n  method: post\n  operationId: createRecognition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recognitions/{id}\n  method: get\n  operationId: getRecognition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recognitions/{id}/confirm\n  method: post\n  operationId: confirmRecognition\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /countries\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /accounts\n  method: delete\n  operationId: deleteAnonymousAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sightings\n  method: get\n  operationId: getSightings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sightings\n  method: put\n  operationId: putSightings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /animals/{id}/photo-report\n  method: post\n \
  \ operationId: reportPhoto\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-error\n  method: post\n  operationId: reportClientError\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/animalchecklist-com/agentic-access/animalchecklist-com-agentic-access.yml
summary_line: 41 operations · 23 acting · 1 human-in-the-loop
tags:
- Company
- Animals
- Checklist
- Mobile App
- Free
---
