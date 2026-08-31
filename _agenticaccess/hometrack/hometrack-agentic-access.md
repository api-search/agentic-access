---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 41
api_specs:
- filename: hometrack-authentication-api-openapi.yml
  format: yaml
  label: Hometrack Authentication API
  slug: hometrack-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-authentication-api-openapi.yml
- filename: hometrack-brands-api-openapi.yml
  format: yaml
  label: Hometrack Brands API
  slug: hometrack-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-brands-api-openapi.yml
- filename: hometrack-broker-api-openapi.yml
  format: yaml
  label: Hometrack Broker API
  slug: hometrack-broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-broker-api-openapi.yml
- filename: hometrack-epc-hometrack-api-openapi.yml
  format: yaml
  label: Hometrack Epc Hometrack API
  slug: hometrack-epc-hometrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-epc-hometrack-api-openapi.yml
- filename: hometrack-flood-twinn-api-openapi.yml
  format: yaml
  label: Hometrack Flood Twinn API
  slug: hometrack-flood-twinn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-flood-twinn-api-openapi.yml
- filename: hometrack-ground-coastalerosion-twinn-api-openapi.yml
  format: yaml
  label: Hometrack Ground Coastalerosion Twinn API
  slug: hometrack-ground-coastalerosion-twinn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-ground-coastalerosion-twinn-api-openapi.yml
- filename: hometrack-ground-subsidence-twinn-api-openapi.yml
  format: yaml
  label: Hometrack Ground Subsidence Twinn API
  slug: hometrack-ground-subsidence-twinn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-ground-subsidence-twinn-api-openapi.yml
- filename: hometrack-ground-terrafirma-api-openapi.yml
  format: yaml
  label: Hometrack Ground Terrafirma API
  slug: hometrack-ground-terrafirma-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-ground-terrafirma-api-openapi.yml
- filename: hometrack-internal-api-openapi.yml
  format: yaml
  label: Hometrack Internal API
  slug: hometrack-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-internal-api-openapi.yml
- filename: hometrack-licences-api-openapi.yml
  format: yaml
  label: Hometrack Licences API
  slug: hometrack-licences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-licences-api-openapi.yml
- filename: hometrack-organisation-api-openapi.yml
  format: yaml
  label: Hometrack Organisation API
  slug: hometrack-organisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-organisation-api-openapi.yml
- filename: hometrack-partners-api-openapi.yml
  format: yaml
  label: Hometrack Partners API
  slug: hometrack-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-partners-api-openapi.yml
- filename: hometrack-pvrplugin-api-openapi.yml
  format: yaml
  label: Hometrack Pvrplugin API
  slug: hometrack-pvrplugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-pvrplugin-api-openapi.yml
- filename: hometrack-reporting-api-openapi.yml
  format: yaml
  label: Hometrack Reporting API
  slug: hometrack-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-reporting-api-openapi.yml
- filename: hometrack-status-api-openapi.yml
  format: yaml
  label: Hometrack Status API
  slug: hometrack-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-status-api-openapi.yml
- filename: hometrack-trial-api-openapi.yml
  format: yaml
  label: Hometrack Trial API
  slug: hometrack-trial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-trial-api-openapi.yml
- filename: hometrack-valuation-api-openapi.yml
  format: yaml
  label: Hometrack Valuation API
  slug: hometrack-valuation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-valuation-api-openapi.yml
- filename: hometrack-zoopla-api-openapi.yml
  format: yaml
  label: Hometrack Zoopla API
  slug: hometrack-zoopla-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-zoopla-api-openapi.yml
consequence_counts:
  physical: 4
  read: 41
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hometrack Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/pvrplugin/enquiry/{token}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/pvrplugin/order/{token}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /broker/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /broker/v2/order
operation_count: 59
overview: 'Hometrack exposes 59 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 41 read, 14 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hometrack
provider_slug: hometrack
slug: hometrack-agentic-access
source_filename: hometrack-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/hometrack-api-public-openapi.yml, openapi/hometrack-broker-avm-api-openapi.yml,\n  openapi/hometrack-climate-api-v2-openapi.yml, openapi/hometrack-prh-core-external-client-api-v2-openapi.yml,\n  openapi/hometrack-valuation-api-v1-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 59\n  by_action_class:\n    acting: 18\n    connected: 41\n  by_consequence:\n    write: 14\n    read: 41\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/authentication/{apiKey}\n  method: post\n  operationId: AuthenticationApi_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reporting/moveToBlobStorage\n  method: get\n  operationId: ReportingApi_MoveToBlobStorage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pvrplugin/enquiry/{token}\n  method: post\n  operationId: PvrPluginApi_StoreEnquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/zoopla/partners/{token}\n  method: post\n  operationId: ZooplaPartnersApi_CreateZooplaPartner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/partners/{token}\n  method: post\n  operationId: PartnersApi_Post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pvrplugin/order/{token}\n  method: post\n  operationId: PvrPluginApi_GenerateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/brands/{token}/{targetAccountApiKey}\n\
  \  method: put\n  operationId: BrandsApi_Put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/brands/{token}/{targetAccountApiKey}\n  method: get\n  operationId: BrandsApi_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reporting/PropertyValuation/{token}/{transactionReference}\n  method: get\n  operationId: ReportingApi_RetrievePropertyValuationReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reporting/TestGet\n  method: get\n  operationId: ReportingApi_TestGet\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reporting/TestPost\n  method: post\n  operationId: ReportingApi_TestPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reporting/PropertyValuation\n  method: post\n  operationId: ReportingApi_RequestPropertyValuationReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reporting/PropertyValuation/config/{token}\n  method: get\n  operationId: ReportingApi_GetPvrConfigurations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/partners/{token}/{partnerType}/{id}\n  method: get\n  operationId: PartnersApi_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/licences/{token}/{product}\n  method: get\n  operationId: LicencesApi_Licences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pvrplugin/{domain}\n  method: get\n  operationId: PvrPluginApi_GetConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pvrplugin/{domain}/{partnerid}\n  method: get\n  operationId: PvrPluginApi_GetConfigurationByPartnerId\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/trial/{apikey}/{token}\n  method: get\n  operationId: TrialApi_Trial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reporting/{token}\n  method: post\n  operationId: ReportingApi_ProcessPropertyValuation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/trial/{token}\n  method: post\n  operationId: TrialApi_NewTrial\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /broker/valuation/{valuationId}\n  method: get\n  operationId: FindValuationById-Spec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/v2/valuation/{valuationId}\n  method: get\n  operationId: FindValuationByIdV2-Spec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal/valuation/{valuationId}/raw\n  method: get\n  operationId: GetRawValuationById-Spec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internal/v2/valuation/{valuationId}/raw\n  method: get\n  operationId: GetRawValuationByIdV2-Spec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/valuation/{valuationId}/input\n  method: get\n  operationId: GetValuationInputById-Spec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/v2/valuation/{valuationId}/input\n  method: get\n  operationId: GetValuationInputByIdV2-Spec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/order/{orderId}\n  method: get\n  operationId: GetValuationOrderById-Spec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/v2/order/{orderId}\n  method: get\n  operationId: GetValuationOrderByIdV2-Spec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /broker/order/{orderId}/status\n  method: get\n  operationId: GetValuationStatusById-Spec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/v2/order/{orderId}/status\n  method: get\n  operationId: GetValuationStatusByIdV2-Spec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /broker/order\n  method: post\n  operationId: ValuePropertyBroker-Spec\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /broker/v2/order\n  method: post\n  operationId:\
  \ ValuePropertyBrokerV2-Spec\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ground-coastalerosion-twinn/{uprn}\n  method: get\n  operationId: CoastalErosionData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /epc-hometrack/{uprn}\n  method: get\n  operationId: Epc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flood-twinn/{uprn}\n  method: get\n  operationId: Flood\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /ground-terrafirma/{uprn}\n  method: get\n  operationId: Ground\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ground-subsidence-twinn/{uprn}\n  method: get\n  operationId: SubsidenceScoreData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case\n  method: get\n  operationId: get-organisation-orgid-case\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case/{caseId}\n  method: get\n  operationId: get-organisation-orgid-case-caseid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case/{caseId}/documents\n\
  \  method: get\n  operationId: get-organisation-orgid-case-caseid-documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case/{caseId}/documents\n  method: post\n  operationId: post-organisation-orgid-case-caseid-documents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/{orgId}/case/{caseId}/documents/{documentReference}\n  method: get\n  operationId: get-organisation-orgid-case-caseid-documents-documentreference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case/{caseId}/documents/{documentReference}/verify\n\
  \  method: get\n  operationId: get-organisation-orgid-case-caseid-documents-documentreference-verify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case/{caseId}/process/{caseProcessId}\n  method: get\n  operationId: get-organisation-orgid-case-caseid-process-caseprocessid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case/{caseId}/process/{caseProcessId}/status\n  method: get\n  operationId: get-organisation-orgid-case-caseid-process-caseprocessid-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case/{caseId}/report\n  method: get\n  operationId: get-organisation-orgid-case-caseid-report\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case/{caseId}/report/{revision}\n  method: get\n  operationId: get-organisation-orgid-case-caseid-report-revision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case/{caseId}/report/latest\n  method: get\n  operationId: get-organisation-orgid-case-caseid-report-latest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case/{caseId}/status\n  method: get\n  operationId: get-organisation-orgid-case-caseid-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/case/{caseId}/status\n\
  \  method: post\n  operationId: post-organisation-orgid-case-caseid-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/{orgId}/case/{caseId}/status/latest\n  method: get\n  operationId: get-organisation-orgid-case-caseid-status-latest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/instruction\n  method: post\n  operationId: post-organisation-orgid-instruction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /organisation/{orgId}/instruction\n  method: put\n  operationId: put-organisation-orgid-instruction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organisation/{orgId}/property/repository\n  method: get\n  operationId: get-organisation-orgid-property-repository\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/property/repository/{repositoryId}\n  method: get\n  operationId: get-organisation-orgid-property-repository-repositoryid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisation/{orgId}/property\n\
  \  method: get\n  operationId: get-organisation-orgid-property-postalcode-postalcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authentication/{apiKey}\n  method: post\n  operationId: authentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valuation/{accountId}\n  method: post\n  operationId: valuation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/agentic-access/hometrack-agentic-access.yml
summary_line: 59 operations · 18 acting
tags:
- Real-Estate
- United Kingdom
- PropTech
- Valuation
- AVM
- Mortgage
- Property Data
- Climate Risk
- Lending
- Surveying
---
