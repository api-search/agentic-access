---
acting_count: 84
action_class_counts:
  acting: 84
  connected: 121
api_specs:
- filename: form3-payments.yml
  format: yaml
  label: Form3 Public API
  slug: form3-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Payments API
  slug: form3-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Direct Debits & Mandates API
  slug: form3-direct-debits-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Account Identification & Verification API
  slug: form3-account-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Files API
  slug: form3-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Event Notifications API
  slug: form3-event-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
- filename: form3-payments.yml
  format: yaml
  label: Form3 Security & Access API
  slug: form3-security-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/openapi/form3-payments.yml
consequence_counts:
  physical: 18
  read: 121
  safety-critical: 2
  write: 64
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Form3 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /security/roles/{role_id}/aces
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /security/roles/{role_id}/aces/{ace_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /transaction/payments/{id}/admissions/{admissionId}/tasks/{taskId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/advices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/advices/{adviceId}/submissions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/recalls
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/recalls/{recallId}/decisions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/recalls/{recallId}/decisions/{decisionId}/submissions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/recalls/{recallId}/submissions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/returns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/returns/{returnId}/reversals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/returns/{returnId}/submissions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/reversals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /transaction/payments/{id}/reversals/{reversalId}/admissions/{admissionId}/tasks/{taskId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/reversals/{reversalId}/submissions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/payments/{id}/submissions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /transaction/payments/{id}/submissions/{submissionId}/tasks/{taskId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /transaction/payments/{paymentId}/returns/{returnId}/admissions/{returnAdmissionId}/tasks/{taskId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /transaction/payments/{paymentId}/returns/{returnId}/submissions/{returnSubmissionId}/tasks/{taskId}
operation_count: 205
overview: 'Form3 exposes 205 API operations that an AI agent could call, of which 84 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 121 read, 64 write, 18 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Form3
provider_slug: form3
slug: form3-agentic-access
source_filename: form3-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/form3-payments.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 205\n  by_action_class:\n    connected: 121\n    acting: 84\n  by_consequence:\n    read: 121\n    write: 64\n    safety-critical: 2\n    physical: 18\n  human_in_the_loop_required: 2\noperations:\n- path: /audit/entries/{record_type}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit/entries/{record_type}/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/schemefiles\n\
  \  method: get\n  operationId: ListSchemeFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/schemefiles\n  method: post\n  operationId: CreateSchemeFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/schemefiles/{scheme_file_id}\n  method: get\n  operationId: GetSchemeFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/schemefiles/{scheme_file_id}\n  method: put\n  operationId: UploadSchemeFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/schemefiles/{scheme_file_id}/admissions\n  method: post\n  operationId: CreateSchemeFileAdmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/schemefiles/{scheme_file_id}/admissions/{scheme_file_admission_id}\n  method: get\n  operationId: GetSchemeFileAdmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/schemefiles/{scheme_file_id}/submissions\n  method: post\n  operationId: CreateSchemeFileSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/schemefiles/{scheme_file_id}/submissions/{scheme_file_submission_id}\n  method: get\n  operationId: GetSchemeFileSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/transactions\n  method: get\n  operationId: ListTransactionFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/transactions\n  method: post\n  operationId: CreateTransactionFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/transactions/{transaction_file_id}\n  method: get\n  operationId: GetTransactionFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/transactions/{transaction_file_id}\n  method: put\n  operationId: UploadTransactionFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/transactions/{transaction_file_id}/admissions\n  method: post\n  operationId: CreateTransactionFileAdmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/transactions/{transaction_file_id}/admissions/{transaction_file_admission_id}\n  method: get\n  operationId: GetTransactionFileAdmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/transactions/{transaction_file_id}/submissions\n  method: post\n  operationId: CreateTransactionFileSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/transactions/{transaction_file_id}/submissions/{transaction_file_submission_id}\n  method: get\n  operationId: GetTransactionFileSubmission\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/transactions/{transaction_file_id}/submissions/{transaction_file_submission_id}/tasks/{task_id}\n  method: get\n  operationId: GetTransactionFileSubmissionTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/transactions/{transaction_file_id}/submissions/{transaction_file_submission_id}/tasks/{task_id}\n  method: patch\n  operationId: PatchTransactionFileSubmissionTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics/prometheus/api/v1/query\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/prometheus/api/v1/query\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics/prometheus/api/v1/query_range\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/prometheus/api/v1/query_range\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics/prometheus/federate\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notification/reports\n  method: get\n  operationId: ListReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notification/reports/{id}\n  method: get\n  operationId: GetReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notification/reports/{id}/admissions/{admissionId}\n  method: get\n  operationId: GetReportAdmissionByID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notification/reports/{id}/content\n  method: get\n  operationId: GetReportContent\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notification/schememessages\n  method: get\n  operationId: ListMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notification/schememessages/{id}\n  method: get\n  operationId: FetchMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notification/schememessages/{id}/admissions/{admissionId}\n  method: get\n  operationId: GetSchemeMessageAdmissionByAdmissionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notification/subscriptions\n  method: get\n  operationId: ListSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notification/subscriptions\n  method: post\n  operationId: CreateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notification/subscriptions/{id}\n  method: delete\n  operationId: DeleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notification/subscriptions/{id}\n  method: get\n  operationId: FetchSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /notification/subscriptions/{id}\n  method: patch\n  operationId: PatchSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/accounts\n  method: get\n  operationId: ListAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/accounts\n  method:\
  \ post\n  operationId: CreateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/accounts/{account_id}/identifications\n  method: get\n  operationId: ListAccountIdentificationsByAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/accounts/{account_id}/identifications\n  method: post\n  operationId: CreateAccountIdentification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/accounts/{account_id}/identifications/{identification_id}\n\
  \  method: delete\n  operationId: DeleteAccountIdentification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/accounts/{account_id}/identifications/{identification_id}\n  method: get\n  operationId: GetAccountIdentification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/accounts/{account_id}/identifications/{identification_id}\n  method: patch\n  operationId: PatchAccountIdentification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /organisation/accounts/{id}\n  method: delete\n  operationId: DeleteAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/accounts/{id}\n  method: get\n  operationId: GetAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/accounts/{id}\n  method: patch\n  operationId: PatchAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/accounts/{id}/events\n\
  \  method: get\n  operationId: GetAccountEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/branches\n  method: get\n  operationId: ListBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/branches\n  method: post\n  operationId: CreateBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/branches/{branch_id}/identifications\n  method: get\n  operationId: ListBranchIdentificationsByBranch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /organisation/branches/{branch_id}/identifications\n  method: post\n  operationId: CreateBranchIdentification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/branches/{branch_id}/identifications/{identification_id}\n  method: delete\n  operationId: DeleteBranchIdentification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/branches/{branch_id}/identifications/{identification_id}\n  method: get\n  operationId: GetBranchIdentification\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/branches/{branch_id}/identifications/{identification_id}\n  method: patch\n  operationId: PatchBranchIdentification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/branches/{id}\n  method: delete\n  operationId: DeleteBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/branches/{id}\n  method: get\n  operationId: GetBranch\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/branches/{id}\n  method: patch\n  operationId: PatchBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/nameverifications\n  method: get\n  operationId: ListNameVerifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/nameverifications\n  method: post\n  operationId: CreateNameVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/nameverifications/{id}\n  method: get\n  operationId: GetNameVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/nameverifications/{name_verification_id}/admissions/{id}\n  method: get\n  operationId: GetNameVerificationAdmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/positions\n  method: get\n  operationId: ListPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/units\n  method: get\n  operationId: ListAllOrganisations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/units\n  method: post\n  operationId: CreateOrganisation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/units/{id}\n  method: get\n  operationId: FetchOrganisation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/units/{id}\n  method: patch\n  operationId: UpdateOrganisation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /platform/security/signing_keys\n  method: get\n  operationId: ListSigningKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platform/security/signing_keys/{signingkey_id}\n  method: get\n  operationId: GetSigningKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/roles\n  method: get\n  operationId: ListAllRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/roles\n  method: post\n  operationId: CreateRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /security/roles/{role_id}\n  method: delete\n  operationId: DeleteRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/roles/{role_id}\n  method: get\n  operationId: FetchRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/roles/{role_id}/aces\n  method: get\n  operationId: ListAllAccessControlsForRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/roles/{role_id}/aces\n  method: post\n  operationId: CreateAccessControlEntry\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /security/roles/{role_id}/aces/{ace_id}\n  method: delete\n  operationId: DeleteAccessControlEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /security/roles/{role_id}/aces/{ace_id}\n  method: get\n  operationId: FetchAccessControlEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/users\n  method:\
  \ get\n  operationId: ListAllUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/users\n  method: post\n  operationId: CreateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/users/{user_id}\n  method: delete\n  operationId: DeleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/users/{user_id}\n  method: get\n  operationId: FetchUser\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/users/{user_id}\n  method: patch\n  operationId: UpdateUserDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/users/{user_id}/aces\n  method: get\n  operationId: FetchAccessControlListForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/users/{user_id}/authn/public_keys\n  method: get\n  operationId: ListPublicKeysForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/users/{user_id}/authn/public_keys\n\
  \  method: post\n  operationId: CreatePublicKeyForUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/users/{user_id}/authn/public_keys/{public_key_id}\n  method: get\n  operationId: FetchPublicKeyForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/users/{user_id}/authn/public_keys/{public_key_id}/cancel_deletion\n  method: post\n  operationId: CancelPublicKeyDeletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /security/users/{user_id}/authn/public_keys/{public_key_id}/schedule_deletion\n  method: post\n  operationId: SchedulePublicKeyDeletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/users/{user_id}/credentials\n  method: get\n  operationId: FetchCredentialsForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/users/{user_id}/credentials\n  method: post\n  operationId: CreateNewCredentialsForUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/users/{user_id}/credentials/{client_id}\n  method: delete\n  operationId: DeleteCredentialsForUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/users/{user_id}/roles\n  method: get\n  operationId: FetchAllRolesForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/users/{user_id}/roles/{role_id}\n  method: delete\n  operationId: RemoveRoleFromUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/users/{user_id}/roles/{role_id}\n  method: post\n  operationId: AddRoleToUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/claims\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/claims\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/claims/{id}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/claims/{id}/reversals\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/claims/{id}/reversals/{reversalId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/claims/{id}/reversals/{reversalId}/submissions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/claims/{id}/reversals/{reversalId}/submissions/{submissionId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/claims/{id}/submissions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/claims/{id}/submissions/{submissionId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/directdebits\n  method: get\n  operationId: GetDirectdebits\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/directdebits\n  method: post\n  operationId: PostDirectdebits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/directdebits/{id}\n  method: get\n  operationId: GetDirectdebitsID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/directdebits/{id}/admissions/{admissionId}\n  method: get\n  operationId: GetDirectdebitsIDAdmissionsAdmissionID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/directdebits/{id}/decisions\n\
  \  method: post\n  operationId: PostDirectdebitsIDDecisions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/directdebits/{id}/decisions/{decisionId}\n  method: get\n  operationId: GetDirectdebitsIDDecisionsDecisionID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/directdebits/{id}/decisions/{decisionId}/admissions/{admissionId}\n  method: get\n  operationId: GetDirectdebitsIDDecisionsDecisionIDAdmissionsAdmissionID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/dire\n\n# --- truncated at 32 KB (61 KB total)\
  \ ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/agentic-access/form3-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/form3/refs/heads/main/agentic-access/form3-agentic-access.yml
summary_line: 205 operations · 84 acting · 2 human-in-the-loop
tags:
- Payments
- United Kingdom
- Payment Processing
- Account-to-Account
- Real-Time Payments
- Faster Payments
- Bacs
- SEPA
- Direct Debit
- Confirmation of Payee
- Cross-Border
- Banking-as-a-Service
- Embedded Payments
---
