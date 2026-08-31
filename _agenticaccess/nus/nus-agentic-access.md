---
acting_count: 0
action_class_counts:
  connected: 5
  privileged: 3
api_specs:
- filename: nus-authorization-api-openapi.yml
  format: yaml
  label: National University of Singapore Authorization API
  slug: nus-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/openapi/nus-authorization-api-openapi.yml
- filename: nus-discovery-api-openapi.yml
  format: yaml
  label: National University of Singapore Discovery API
  slug: nus-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/openapi/nus-discovery-api-openapi.yml
- filename: nus-session-api-openapi.yml
  format: yaml
  label: National University of Singapore Session API
  slug: nus-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/openapi/nus-session-api-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts for the one institution-operated National University of Singapore API surface, classified from the contract in openapi/. This replaces an earlier version of this file that was derived from the NUSMods API — a student organisation's contract, not NUS's — and therefore credited NUS with someone else's engineering. A governance starting point; review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: derived
name: Nus Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'National University of Singapore exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: National University of Singapore
provider_slug: nus
slug: nus-agentic-access
source_filename: nus-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: derived\nsource: openapi/nus-identity-openapi.yml\nx-operator: institution\ndescription: >-\n  Recommended x-agentic-access execution contracts for the one institution-operated National\n  University of Singapore API surface, classified from the contract in openapi/. This replaces\n  an earlier version of this file that was derived from the NUSMods API — a student\n  organisation's contract, not NUS's — and therefore credited NUS with someone else's\n  engineering. A governance starting point; review and bind audience per deployment.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 5\n    privileged: 3\n  by_consequence:\n    read: 5\n    write: 3\n  human_in_the_loop_required: 3\ncaveat: >-\n  This is an identity provider. Every write-consequence operation here mints or terminates\n  credentials for a real person at a real university. No agent should hold a client_secret for\n  this\
  \ provider without an explicit, auditable institutional grant from NUS Information\n  Technology, and NUS operates no self-service path to obtain one.\noperations:\n- path: /adfs/.well-known/openid-configuration\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: null\n    audit: none\n    notes: Public discovery document. Safe for an agent to poll; it is the only change signal NUS emits.\n- path: /adfs/discovery/keys\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: null\n    audit: none\n    notes: Public signing keys. Cache and honour rotation.\n- path: /FederationMetadata/2007-06/FederationMetadata.xml\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: null\n    audit: none\n    notes: Public signed SAML metadata. Verify the signature before trusting it.\n- path: /adfs/oauth2/authorize/\n\
  \  method: get\n  x-agentic-access:\n    action-class: privileged\n    consequence: write\n    subject: required\n    human-in-the-loop: required\n    token:\n      max-ttl: 300\n    audit: full\n    notes: >-\n      Initiates interactive authentication of a real person. An agent must never drive this\n      without the human present; that is the entire point of the endpoint.\n- path: /adfs/oauth2/token/\n  method: post\n  x-agentic-access:\n    action-class: privileged\n    consequence: write\n    subject: required\n    human-in-the-loop: required\n    token:\n      max-ttl: 3600\n    audit: full\n    notes: >-\n      Mints access, refresh and ID tokens. The provider advertises the password and implicit\n      grants; an agent must use neither. Refresh tokens issued here should be treated as\n      credentials of the person, not of the agent.\n- path: /adfs/oauth2/devicecode\n  method: post\n  x-agentic-access:\n    action-class: privileged\n    consequence: write\n    subject: required\n\
  \    human-in-the-loop: required\n    token:\n      max-ttl: 900\n    audit: full\n    notes: Device authorization grant; requires a human to complete verification out of band.\n- path: /adfs/userinfo\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 3600\n    audit: full\n    notes: >-\n      Returns claims about an identified student or staff member. Personal data under\n      Singapore's PDPA; minimise, do not retain, and do not use `sub` as a durable key — it is\n      pairwise and will differ per client.\n- path: /adfs/oauth2/logout\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token: null\n    audit: full\n    notes: Terminates the user's session. Idempotent and safe, but log it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/agentic-access/nus-agentic-access.yml
summary_line: 8 operations · 3 human-in-the-loop
tags:
- University
- Higher Education
- Education
- Singapore
- Research
- Identity Federation
- Research Repository
- Course Catalog
- Open Access
- Learning Management
---
