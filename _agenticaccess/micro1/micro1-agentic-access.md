---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 8
api_specs:
- filename: micro1-interview-api-openapi.yml
  format: yaml
  label: micro1 Interview API
  slug: micro1-interview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-interview-api-openapi.yml
- filename: micro1-interview-reports-api-openapi.yml
  format: yaml
  label: micro1 Interview Reports API
  slug: micro1-interview-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-interview-reports-api-openapi.yml
- filename: micro1-invite-candidate-api-openapi.yml
  format: yaml
  label: micro1 Invite Candidate API
  slug: micro1-invite-candidate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-invite-candidate-api-openapi.yml
- filename: micro1-job-api-openapi.yml
  format: yaml
  label: micro1 Job API
  slug: micro1-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-job-api-openapi.yml
- filename: micro1-job-applicant-api-openapi.yml
  format: yaml
  label: micro1 Job Applicant API
  slug: micro1-job-applicant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-job-applicant-api-openapi.yml
- filename: micro1-webhook-api-openapi.yml
  format: yaml
  label: micro1 Webhook API
  slug: micro1-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/openapi/micro1-webhook-api-openapi.yml
consequence_counts:
  read: 8
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Micro1 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'micro1 exposes 18 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: micro1
provider_slug: micro1
slug: micro1-agentic-access
source_filename: micro1-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: generated\nsource: openapi/micro1-ai-recruiter-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 10\n    connected: 8\n  by_consequence:\n    write: 10\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /interview\n  method: post\n  operationId: aiInterviewer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom/interview\n  method: post\n  operationId: aiInterviewer-ce2743c0-2309-41eb-8ff2-44c55c138c25\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /interviews\n  method: get\n  operationId: aiInterviewer-34586a03-d777-4757-8c54-f8d7e4c821a5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interview/{interviewId}\n  method: put\n  operationId: aiInterviewer-6d5d608a-0b31-460d-80b8-a69aa43aac17\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /interview/{interviewId}\n  method: delete\n  operationId: aiInterviewer-b7d10a6a-f334-4836-933f-c9a62d33d80b\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /interview/invite\n  method: post\n  operationId: aiInterviewer-08720534-ee71-4a6c-aff1-25c48ed78c6d\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /interview/invites\n  method: get\n  operationId: aiInterviewer-f690665f-6248-4c86-b317-0f18ebecf728\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interview/reports\n  method: get\n  operationId: aiInterviewer-c5c30f81-a2b4-45ca-9943-f034683993b0\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interview/recording\n  method: get\n  operationId: aiInterviewer-224f9971-cd82-4432-9f9f-8e4f1ba73345\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mock/interview\n  method: post\n  operationId: aiInterviewer-2bc90237-ae08-40ae-8d61-08907a167e52\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: jobsApplicant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /job/{jobId}/applicant\n  method: post\n  operationId: jobsApplicant-c1ce8fbf-390b-412b-9895-d422b21e823e\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/{jobId}/applicants\n  method: get\n  operationId: jobsApplicant-8934b0b6-90a5-42a4-a5e6-c37d3833718e\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/applicant/{jobApplicantId}\n  method: get\n  operationId: jobsApplicant-e3619770-a47f-4349-838d-a612736b5621\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook\n  method: post\n  operationId: webhookSetup\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: webhookSetup-51ac71f1-e1da-425d-afa2-d527e716b7e6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/{webhookId}\n  method: put\n  operationId: webhookSetup-c050afb6-e424-4a49-81a7-839386c17724\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/{webhookId}\n  method: delete\n  operationId: webhookSetup-223f3d34-faeb-4c70-91df-a08a2baa2141\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/micro1/refs/heads/main/agentic-access/micro1-agentic-access.yml
summary_line: 18 operations · 10 acting
tags:
- Company
- Recruiting
- Hiring
- AI Interviews
- Talent Assessment
- Candidate Screening
- Applicant Tracking
- Human Resources
- Proctoring
- Webhook
- agent-native
- AI Training Data
---
