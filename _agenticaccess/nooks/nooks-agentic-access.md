---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 24
api_specs:
- filename: nooks-accounts-api-openapi.yml
  format: yaml
  label: Nooks Accounts API
  slug: nooks-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-accounts-api-openapi.yml
- filename: nooks-calldispositions-api-openapi.yml
  format: yaml
  label: Nooks Call Dispositions API
  slug: nooks-calldispositions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-calldispositions-api-openapi.yml
- filename: nooks-calls-api-openapi.yml
  format: yaml
  label: Nooks Calls API
  slug: nooks-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-calls-api-openapi.yml
- filename: nooks-emails-api-openapi.yml
  format: yaml
  label: Nooks Emails API
  slug: nooks-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-emails-api-openapi.yml
- filename: nooks-emailtemplates-api-openapi.yml
  format: yaml
  label: Nooks Email Templates API
  slug: nooks-emailtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-emailtemplates-api-openapi.yml
- filename: nooks-introspection-api-openapi.yml
  format: yaml
  label: Nooks Introspection API
  slug: nooks-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-introspection-api-openapi.yml
- filename: nooks-mailboxes-api-openapi.yml
  format: yaml
  label: Nooks Mailboxes API
  slug: nooks-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-mailboxes-api-openapi.yml
- filename: nooks-nooks-sequencing-api-api-openapi.yml
  format: yaml
  label: Nooks Nooks Sequencing API
  slug: nooks-nooks-sequencing-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-nooks-sequencing-api-api-openapi.yml
- filename: nooks-notes-api-openapi.yml
  format: yaml
  label: Nooks Notes API
  slug: nooks-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-notes-api-openapi.yml
- filename: nooks-prospects-api-openapi.yml
  format: yaml
  label: Nooks Prospects API
  slug: nooks-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-prospects-api-openapi.yml
- filename: nooks-sequences-api-openapi.yml
  format: yaml
  label: Nooks Sequences API
  slug: nooks-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequences-api-openapi.yml
- filename: nooks-sequencestates-api-openapi.yml
  format: yaml
  label: Nooks Sequence States API
  slug: nooks-sequencestates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequencestates-api-openapi.yml
- filename: nooks-sequencesteps-api-openapi.yml
  format: yaml
  label: Nooks Sequence Steps API
  slug: nooks-sequencesteps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequencesteps-api-openapi.yml
- filename: nooks-tasks-api-openapi.yml
  format: yaml
  label: Nooks Tasks API
  slug: nooks-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-tasks-api-openapi.yml
- filename: nooks-users-api-openapi.yml
  format: yaml
  label: Nooks Users API
  slug: nooks-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-users-api-openapi.yml
consequence_counts:
  read: 24
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nooks Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: 'Nooks exposes 37 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nooks
provider_slug: nooks
slug: nooks-agentic-access
source_filename: nooks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/nooks-sequencing-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 24\n    acting: 13\n  by_consequence:\n    read: 24\n    write: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /sequences\n  method: get\n  operationId: listSequences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences\n  method: post\n  operationId: createSequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/{id}\n  method: get\n  operationId: getSequence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/{id}\n  method: patch\n  operationId: updateSequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequenceSteps\n  method: get\n  operationId: listSequenceSteps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequenceSteps/{id}\n  method: get\n  operationId: getSequenceStep\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emailTemplate/{id}\n  method: get\n  operationId: getEmailTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequenceStates\n  method: get\n  operationId: listSequenceStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequenceStates\n  method: post\n  operationId:\
  \ createSequenceState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequenceStates/{id}\n  method: get\n  operationId: getSequenceState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequenceStates/{id}\n  method: delete\n  operationId: deleteSequenceState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequenceStates/{id}/actions/finish\n  method: post\n  operationId: finishSequenceState\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prospects\n  method: get\n  operationId: listProspects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/prospects/sync\n  method: post\n  operationId: syncProspects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prospects/{id}\n  method: get\n  operationId: getProspect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /prospects/{id}/notes\n  method: post\n  operationId: createProspectNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}/notes\n  method: post\n  operationId: createAccountNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailboxes\n  method: get\n  operationId: listMailboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailboxes/{id}\n  method: get\n  operationId: getMailbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails\n  method: get\n  operationId: listEmails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emails/{id}\n  method: get\n  operationId: getEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /calls\n  method: get\n  operationId: listCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/{id}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /callDispositions\n  method: get\n  operationId: listCallDispositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /callDispositions/{id}\n  method: get\n  operationId: getCallDisposition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks\n  method: post\n  operationId: createTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}\n  method: get\n  operationId: getTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{id}\n  method: patch\n  operationId: updateTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}\n  method: delete\n  operationId:\
  \ deleteTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}/complete\n  method: post\n  operationId: completeTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}/skip\n  method: post\n  operationId: skipTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n\
  \  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/agentic-access/nooks-agentic-access.yml
summary_line: 37 operations · 13 acting
tags:
- Company
- Artificial Intelligence
- Sales Engagement
- Sales Dialer
- AI SDR
- Outbound Sales
- Sales Coaching
- Revenue Operations
- Sales Sequencing
- CRM Integration
- Agents
- MCP
---
