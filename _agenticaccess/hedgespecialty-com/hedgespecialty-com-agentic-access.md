---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 46
api_specs:
- filename: hedgespecialty-com-account-api-openapi.yml
  format: yaml
  label: Hedge Account API
  slug: hedgespecialty-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-account-api-openapi.yml
- filename: hedgespecialty-com-appetite-api-openapi.yml
  format: yaml
  label: Hedge Appetite API
  slug: hedgespecialty-com-appetite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-appetite-api-openapi.yml
- filename: hedgespecialty-com-auth-api-openapi.yml
  format: yaml
  label: Hedge Auth API
  slug: hedgespecialty-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-auth-api-openapi.yml
- filename: hedgespecialty-com-binding-api-openapi.yml
  format: yaml
  label: Hedge Binding API
  slug: hedgespecialty-com-binding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-binding-api-openapi.yml
- filename: hedgespecialty-com-carrier-quotes-api-openapi.yml
  format: yaml
  label: Hedge Carrier quotes API
  slug: hedgespecialty-com-carrier-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-carrier-quotes-api-openapi.yml
- filename: hedgespecialty-com-documents-api-openapi.yml
  format: yaml
  label: Hedge Documents API
  slug: hedgespecialty-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-documents-api-openapi.yml
- filename: hedgespecialty-com-market-access-api-openapi.yml
  format: yaml
  label: Hedge Market access API
  slug: hedgespecialty-com-market-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-market-access-api-openapi.yml
- filename: hedgespecialty-com-payments-api-openapi.yml
  format: yaml
  label: Hedge Payments API
  slug: hedgespecialty-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-payments-api-openapi.yml
- filename: hedgespecialty-com-policies-api-openapi.yml
  format: yaml
  label: Hedge Policies API
  slug: hedgespecialty-com-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-policies-api-openapi.yml
- filename: hedgespecialty-com-programs-api-openapi.yml
  format: yaml
  label: Hedge Programs API
  slug: hedgespecialty-com-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-programs-api-openapi.yml
- filename: hedgespecialty-com-requirements-api-openapi.yml
  format: yaml
  label: Hedge Requirements API
  slug: hedgespecialty-com-requirements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-requirements-api-openapi.yml
- filename: hedgespecialty-com-submissions-api-openapi.yml
  format: yaml
  label: Hedge Submissions API
  slug: hedgespecialty-com-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-submissions-api-openapi.yml
- filename: hedgespecialty-com-webhooks-api-openapi.yml
  format: yaml
  label: Hedge Webhooks API
  slug: hedgespecialty-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgespecialty-com/openapi/hedgespecialty-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 46
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hedgespecialty Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /broker/intake
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /broker/submissions/{submission_id}/withdraw
operation_count: 75
overview: 'Hedge exposes 75 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 46 read, 27 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hedge
provider_slug: hedgespecialty-com
slug: hedgespecialty-com-agentic-access
source_filename: hedgespecialty-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/hedgespecialty-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 75\n  by_action_class:\n    acting: 29\n    connected: 46\n  by_consequence:\n    write: 27\n    read: 46\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/register\n  method: post\n  operationId: registerOAuthClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/authorize\n  method: get\n  operationId: startOAuthAuthorization\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/device_authorization\n  method: post\n  operationId: startOAuthDeviceAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: exchangeOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/me\n  method: get\n  operationId: getBrokerIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions\n  method: get\n  operationId: listSubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions\n  method: post\n  operationId: createSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/intake\n  method: post\n  operationId: intakeSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/markets\n  method: get\n  operationId: getSubmissionMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/quotes\n  method: get\n  operationId: getSubmissionQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/partner-bind-links\n  method: post\n  operationId: createPartnerBindLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}\n  method: get\n  operationId:\
  \ getSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/events\n  method: get\n  operationId: listSubmissionEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/thread\n  method: get\n  operationId: getSubmissionThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/thread\n  method: post\n  operationId: replyToSubmissionThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/documents\n  method: post\n  operationId: uploadSubmissionDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/forms\n  method: get\n  operationId: listBlankApplicationForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/forms/supplementals.zip\n  method: get\n  operationId: downloadAllHedgeSupplementals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/forms/{form_key}/pdf\n  method: get\n  operationId: downloadBlankApplicationForm\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/finalized-documents\n  method: get\n  operationId: listSubmissionDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/finalized-documents/{document_id}/pdf\n  method: get\n  operationId: downloadSubmissionDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/package\n  method: get\n  operationId: getSubmissionPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/package/download\n  method: post\n\
  \  operationId: downloadSubmissionPackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/source-offers/{presentation_id}/original\n  method: get\n  operationId: downloadCarrierOriginalOffer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/requirements\n  method: get\n  operationId: getSubmissionRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/market-rail\n  method: get\n  operationId: getSubmissionMarketRail\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/appetite-preview\n  method: get\n  operationId: getSubmissionAppetitePreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/market-exclusions\n  method: put\n  operationId: setSubmissionMarketExclusions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/form-fill-session\n  method: post\n  operationId: startFormFillSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/api-quotes/sessions\n  method: get\n  operationId: listCarrierQuoteSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/api-quotes/sessions/{session_id}/answers\n  method: post\n  operationId: saveCarrierAnswers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/api-quotes/sessions/{session_id}/close\n  method: post\n  operationId: requestCarrierQuote\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/application-workspace\n  method: get\n  operationId: getApplicationWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/application-workspace/changes\n  method: get\n  operationId: streamApplicationWorkspaceChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/application-workspace/quote-products\n  method: put\n  operationId: setApplicationQuoteProducts\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/application-workspace/add-ons\n  method: post\n  operationId: chooseApplicationAddOn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/applications/{session_id}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/applications/{session_id}/checkpoint\n  method:\
  \ post\n  operationId: checkpointApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/applications/{session_id}/request-quote\n  method: post\n  operationId: requestApplicationQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/applications/{session_id}/business-descriptions\n  method: get\n  operationId: listBusinessDescriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/applications/{session_id}/business-descriptions/search\n  method: get\n  operationId: searchBusinessDescriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/applications/{session_id}/employers-classes\n  method: get\n  operationId: listEmployersClasses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/finalize\n  method: post\n  operationId: finalizeSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /broker/submissions/{submission_id}/outstanding-requirements\n  method: get\n  operationId: getOutstandingRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/asks\n  method: get\n  operationId: getSubmissionAsks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/outstanding-requirements/answers\n  method: post\n  operationId: answerOutstandingRequirements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/answers\n\
  \  method: post\n  operationId: recordPartnerAnswers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/withdraw\n  method: post\n  operationId: withdrawSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/bind-readiness\n  method: get\n  operationId: getBindReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /broker/insureds\n  method: get\n  operationId: listInsureds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/insureds/{insured_id}\n  method: get\n  operationId: getInsured\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/policies\n  method: get\n  operationId: listPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/policies/{policy_id}\n  method: get\n  operationId: getPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/policies/{policy_id}/document/{kind}\n  method: get\n  operationId: downloadPolicyDocument\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/bind-requests\n  method: post\n  operationId: createBindRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/bind-requests\n  method: get\n  operationId: listBindRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/bind-requests/{bind_request_id}\n  method: get\n  operationId: getBindRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/submissions/{submission_id}/bind-requests/{bind_request_id}/contingencies/{contingency_id}/document\n  method: post\n  operationId: uploadBindContingencyDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/submissions/{submission_id}/bind-requests/{bind_request_id}/submit\n  method: post\n  operationId: submitBindRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/appetite\n  method: get\n  operationId: checkAppetite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/appetite/search\n  method: post\n  operationId: searchPlacements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/catalog/query\n  method: post\n  operationId: queryMarketCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/hedge-questions\n  method: post\n  operationId: getHedgeQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /broker/appetite/guide\n  method: get\n  operationId: downloadAppetiteGuide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/markets/{market_id}/requirements\n  method: get\n  operationId: getMarketRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/market-access\n  method: get\n  operationId: getMarketAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/market-access\n  method: put\n  operationId: setMarketAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/market-access/program\n  method: put\n  operationId: setProgramAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/market-access/program-line\n  method: put\n  operationId: setProgramLineAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/market-connections\n  method: get\n  operationId: listMarketConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/market-connections/next-insurance\n  method: put\n  operationId: connectNextInsurance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/market-connections/next-insurance\n  method: delete\n  operationId: disconnectNextInsurance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/programs\n  method: get\n  operationId: listPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /broker/programs/{program_id}/application-schema\n  method: get\n  operationId: getProgramApplicationSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/hedgespecialty-com/agentic-access/hedgespecialty-com-agentic-access.yml
summary_line: 75 operations · 29 acting
tags:
- Company
- Insurance
- Wholesale
- Brokers
- Specialty
---
