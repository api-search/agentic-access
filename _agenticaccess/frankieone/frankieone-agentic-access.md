---
acting_count: 38
action_class_counts:
  acting: 38
  connected: 14
api_specs:
- filename: frankieone-audit-api-openapi.yml
  format: yaml
  label: FrankieOne Audit API
  slug: frankieone-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-audit-api-openapi.yml
- filename: frankieone-hostedurl-api-openapi.yml
  format: yaml
  label: FrankieOne HostedURL API
  slug: frankieone-hostedurl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-hostedurl-api-openapi.yml
- filename: frankieone-idv-api-openapi.yml
  format: yaml
  label: FrankieOne IDV API
  slug: frankieone-idv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-idv-api-openapi.yml
- filename: frankieone-individual-documents-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Documents API
  slug: frankieone-individual-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-documents-api-openapi.yml
- filename: frankieone-individual-entities-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Entities API
  slug: frankieone-individual-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-entities-api-openapi.yml
- filename: frankieone-individual-entity-elements-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Entity Elements API
  slug: frankieone-individual-entity-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-entity-elements-api-openapi.yml
- filename: frankieone-individual-profiles-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Profiles API
  slug: frankieone-individual-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-profiles-api-openapi.yml
- filename: frankieone-individual-results-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Results API
  slug: frankieone-individual-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-results-api-openapi.yml
- filename: frankieone-individual-risks-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Risks API
  slug: frankieone-individual-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-risks-api-openapi.yml
- filename: frankieone-individual-workflows-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Workflows API
  slug: frankieone-individual-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-workflows-api-openapi.yml
- filename: frankieone-matchlists-api-openapi.yml
  format: yaml
  label: FrankieOne Matchlists API
  slug: frankieone-matchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-matchlists-api-openapi.yml
- filename: frankieone-monitoring-api-openapi.yml
  format: yaml
  label: FrankieOne Monitoring API
  slug: frankieone-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-monitoring-api-openapi.yml
- filename: frankieone-search-api-openapi.yml
  format: yaml
  label: FrankieOne Search API
  slug: frankieone-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-search-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  safety-critical: 1
  write: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Frankieone Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v2/individuals/{entityId}/serviceprofiles/{serviceName}/workflows/{workflowName}/executions/{workflowExecutionId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/individuals/{entityId}/consents/{consentType}
operation_count: 52
overview: 'FrankieOne exposes 52 API operations that an AI agent could call, of which 38 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 36 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FrankieOne
provider_slug: frankieone
slug: frankieone-agentic-access
source_filename: frankieone-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/core-v2-openapi.yml, openapi/kyc-v2-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 14\n    acting: 38\n  by_consequence:\n    read: 14\n    write: 36\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v2/audit\n  method: get\n  operationId: listAuditEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/workflows\n  method: get\n  operationId: getWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/search/serviceprofiles\n  method: post\n  operationId: searchProfiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/search/matchlists\n  method: post\n  operationId: searchMatchlists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/matchlists\n  method: get\n  operationId: getMatchlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v2/matchlists/{matchlistName}/entries\n  method: post\n  operationId: createMatchlistEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/matchlists/{matchlistName}/entries\n  method: get\n  operationId: getMatchlistEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/matchlists/{matchlistName}/entries/{entryId}\n  method: patch\n  operationId: updateMatchlistEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/matchlists/{matchlistName}/entries/{entryId}\n  method: get\n  operationId: getMatchlistEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/matchlists/{matchlistName}/entries/addEntity\n  method: post\n  operationId: addMatchlistEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/matchlists/{matchlistName}/entries/removeEntity\n  method: patch\n  operationId: removeMatchlistEntity\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals\n  method: post\n  operationId: createIndividuals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}\n  method: patch\n  operationId: updateIndividual\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v2/individuals/{entityId}\n  method: get\n  operationId: getIndividual\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/individuals/{entityId}\n  method: delete\n  operationId: deleteIndividual\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/workflows\n  method: get\n  operationId: getWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/individuals/new/serviceprofiles/{serviceName}/workflows/{workflowName}/execute\n  method: post\n\
  \  operationId: createAndExecuteWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/serviceprofiles/{serviceName}/workflows/{workflowName}/execute\n  method: post\n  operationId: executeWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/serviceprofiles/{serviceName}/workflows/{workflowName}/executions\n  method: get\n  operationId: getResults\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/individuals/{entityId}/serviceprofiles/{serviceName}/workflows/{workflowName}/executions/{workflowExecutionId}\n  method: get\n  operationId: getWorkflowExecutionResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/individuals/{entityId}/serviceprofiles/{serviceName}/workflows/{workflowName}/executions/{workflowExecutionId}\n  method: patch\n  operationId: overrideWorkflowExecutionResult\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /v2/individuals/{entityId}/serviceprofiles/{serviceName}\n  method: patch\n  operationId: updateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/serviceprofiles/{serviceName}\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/individuals/{entityId}/results/mkyc\n  method: post\n  operationId: manualKYC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/results/mkyc/invalidate\n  method: post\n  operationId: manualKYCinvalidation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/results/aml\n  method: patch\n  operationId: updateAML\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/results/idv\n  method: patch\n  operationId: updateIDV\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/results/matchlist\n  method: patch\n  operationId: updateMatches\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/results/duplicate\n  method: patch\n  operationId: updateDuplicate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/results/fraud\n  method: patch\n  operationId: updateFraud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/results\n  method: get\n  operationId: getAllPROs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/individuals/{entityId}/names/{nameId}\n  method: delete\n  operationId: deleteName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/datesOfBirth/{dateOfBirthId}\n  method: delete\n  operationId: deleteDob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/addresses/{addressId}\n  method: delete\n  operationId: deleteAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/emailaddresses/{emailAddressId}\n\
  \  method: delete\n  operationId: deleteEmailAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/phonenumbers/{phoneNumberId}\n  method: delete\n  operationId: deletePhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/consents/{consentType}\n  method: delete\n  operationId: deleteConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    -\
  \ kyc:api\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/externalreferences\n  method: get\n  operationId: getExternalReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/individuals/{entityId}/externalreferences/{referenceId}\n  method: delete\n  operationId: deleteExternalReference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/search/serviceprofiles\n  method:\
  \ post\n  operationId: searchIndividuals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/documents\n  method: post\n  operationId: createDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/documents\n  method: get\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/individuals/{entityId}/documents/{documentId}\n  method: patch\n  operationId: updateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/documents/{documentId}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - kyc:api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/individuals/{entityId}/documents/{documentId}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/documents/{documentId}/attachments/{attachmentId}\n  method: delete\n  operationId: deleteAttachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/serviceprofiles/{serviceName}/risk\n  method: patch\n  operationId: updateIndividualRiskLevel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/monitor\n\
  \  method: patch\n  operationId: patchMonitoring\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/actions/idv/token\n  method: post\n  operationId: getIDVToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/actions/idv/ocr\n  method: post\n  operationId: processIDVOCR\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/{entityId}/actions/idv/process\n  method: post\n  operationId: initBiometrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/individuals/hostedurl\n  method: post\n  operationId: getHostedUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - kyc:api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/agentic-access/frankieone-agentic-access.yml
summary_line: 52 operations · 38 acting · 1 human-in-the-loop
tags:
- Identity Verification
- KYC
- KYB
- AML
- Fraud
- Compliance
---
