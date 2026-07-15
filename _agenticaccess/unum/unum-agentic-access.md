---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 10
api_specs:
- filename: unum-hr-connect-openapi.yml
  format: yaml
  label: Unum HR Connect API
  slug: hr-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/openapi/unum-hr-connect-openapi.yml
consequence_counts:
  read: 10
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Unum Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /eligibility/members/{memberId}
operation_count: 18
overview: 'Unum exposes 18 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 7 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Unum
provider_slug: unum
slug: unum-agentic-access
source_filename: unum-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/unum-hr-connect-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 8\n    connected: 10\n  by_consequence:\n    write: 7\n    read: 10\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /oauth/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n\
  \    - leave:read\n- path: /eligibility/members\n  method: get\n  operationId: listEligibleMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /eligibility/members\n  method: post\n  operationId: submitMemberEligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /eligibility/members/{memberId}\n  method: get\n  operationId: getMemberEligibility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /eligibility/members/{memberId}\n  method: put\n  operationId: updateMemberEligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /eligibility/members/{memberId}\n  method: delete\n  operationId: terminateMemberEligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /enrollment/elections\n  method: get\n  operationId: listEnrollmentElections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /enrollment/elections\n  method: post\n  operationId: submitEnrollmentElection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n\
  \    - leave:read\n- path: /enrollment/elections/{electionId}\n  method: get\n  operationId: getEnrollmentElection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /leave/requests\n  method: get\n  operationId: listLeaveRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /leave/requests\n  method: post\n  operationId: submitLeaveRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /leave/requests/{requestId}\n  method: get\n  operationId: getLeaveRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /leave/requests/{requestId}\n  method: put\n  operationId: updateLeaveRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path:\
  \ /eoi/submissions\n  method: get\n  operationId: listEoiSubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /eoi/submissions\n  method: post\n  operationId: submitEoi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /eoi/submissions/{submissionId}\n  method: get\n  operationId: getEoiSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /billing/invoices\n  method: get\n  operationId: listBillingInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n- path: /billing/invoices/{invoiceId}\n  method: get\n  operationId: getBillingInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - billing:read\n    - eligibility:read\n    - enrollment:read\n    - eoi:read\n    - leave:read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unum/refs/heads/main/agentic-access/unum-agentic-access.yml
summary_line: 18 operations · 8 acting · 1 human-in-the-loop
tags:
- Insurance
- Benefits Administration
- HR Integration
- Disability Insurance
- Life Insurance
- Fortune 500
---
