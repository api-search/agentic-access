---
acting_count: 102
action_class_counts:
  acting: 102
  connected: 258
api_specs:
- filename: infranest-audit-log-api-openapi.yml
  format: yaml
  label: InfraNest Audit Log API
  slug: infranest-audit-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-audit-log-api-openapi.yml
- filename: infranest-authentication-api-openapi.yml
  format: yaml
  label: InfraNest Authentication API
  slug: infranest-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-authentication-api-openapi.yml
- filename: infranest-automations-api-openapi.yml
  format: yaml
  label: InfraNest Automations API
  slug: infranest-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-automations-api-openapi.yml
- filename: infranest-billing-api-openapi.yml
  format: yaml
  label: InfraNest Billing API
  slug: infranest-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-billing-api-openapi.yml
- filename: infranest-certificates-api-openapi.yml
  format: yaml
  label: InfraNest Certificates API
  slug: infranest-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-certificates-api-openapi.yml
- filename: infranest-cloud-api-openapi.yml
  format: yaml
  label: InfraNest Cloud API
  slug: infranest-cloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-cloud-api-openapi.yml
- filename: infranest-cost-api-openapi.yml
  format: yaml
  label: InfraNest Cost API
  slug: infranest-cost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-cost-api-openapi.yml
- filename: infranest-cost-reporting-api-openapi.yml
  format: yaml
  label: InfraNest Cost reporting API
  slug: infranest-cost-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-cost-reporting-api-openapi.yml
- filename: infranest-custom-fields-api-openapi.yml
  format: yaml
  label: InfraNest Custom fields API
  slug: infranest-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-custom-fields-api-openapi.yml
- filename: infranest-dns-api-openapi.yml
  format: yaml
  label: InfraNest DNS API
  slug: infranest-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-dns-api-openapi.yml
- filename: infranest-domains-api-openapi.yml
  format: yaml
  label: InfraNest Domains API
  slug: infranest-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-domains-api-openapi.yml
- filename: infranest-drop-catch-api-openapi.yml
  format: yaml
  label: InfraNest Drop Catch API
  slug: infranest-drop-catch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-drop-catch-api-openapi.yml
- filename: infranest-dynamic-ip-api-openapi.yml
  format: yaml
  label: InfraNest Dynamic IP API
  slug: infranest-dynamic-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-dynamic-ip-api-openapi.yml
- filename: infranest-endpoints-api-openapi.yml
  format: yaml
  label: InfraNest Endpoints API
  slug: infranest-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-endpoints-api-openapi.yml
- filename: infranest-integration-logs-api-openapi.yml
  format: yaml
  label: InfraNest Integration Logs API
  slug: infranest-integration-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-integration-logs-api-openapi.yml
- filename: infranest-integrations-api-openapi.yml
  format: yaml
  label: InfraNest Integrations API
  slug: infranest-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-integrations-api-openapi.yml
- filename: infranest-monitoring-api-openapi.yml
  format: yaml
  label: InfraNest Monitoring API
  slug: infranest-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-monitoring-api-openapi.yml
- filename: infranest-organizations-api-openapi.yml
  format: yaml
  label: InfraNest Organizations API
  slug: infranest-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-organizations-api-openapi.yml
- filename: infranest-webhooks-api-openapi.yml
  format: yaml
  label: InfraNest Webhooks API
  slug: infranest-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-webhooks-api-openapi.yml
consequence_counts:
  physical: 6
  read: 258
  safety-critical: 15
  write: 81
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 15
kind: agentic-access
layout: agentic-access
method: generated
name: Infranest Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/auth/logout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/alert-rule-overrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/alert-rules/{alertRule_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/alert-rules/{alertRule_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/backup-pricing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/ignored-units
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/pricing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/reset-pricing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/untrack
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/organizations/{organization_id}/deploy-sources
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/organizations/{organization_id}/domains/{domain_id}/archive
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/organizations/{organization_id}/dynamic-ips/{dynamicIp_id}/address
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/organizations/{organization_id}/dynamic-ips/{dynamicIp_id}/agent
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/organizations/{organization_id}/dynamic-ips/{dynamicIp_id}/targets/{target_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/organizations/{organization_id}/sandbox/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/organizations/{organization_id}/deploy-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/organizations/{organization_id}/deploy-links/{deployLink_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/organizations/{organization_id}/dynamic-ips/{dynamicIp_id}/check-in
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/organizations/{organization_id}/dynamic-ips/{dynamicIp_id}/recheck
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/organizations/{organization_id}/status-pages/{statusPage_id}/component-groups/sort
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/organizations/{organization_id}/status-pages/{statusPage_id}/components/sort
operation_count: 360
overview: 'InfraNest exposes 360 API operations that an AI agent could call, of which 102 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 258 read, 81 write, 6 physical, and 15 safety-critical.


  15 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: InfraNest
provider_slug: infranest
slug: infranest-agentic-access
source_filename: infranest-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/infranest-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 360\n  by_action_class:\n    acting: 102\n    connected: 258\n  by_consequence:\n    safety-critical: 15\n    read: 258\n    write: 81\n    physical: 6\n  human_in_the_loop_required: 15\noperations:\n- path: /api/auth/logout\n  method: post\n  operationId: postApiAuthLogout\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/auth/me\n  method:\
  \ get\n  operationId: getApiAuthMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations\n  method: get\n  operationId: getApiOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{id}\n  method: get\n  operationId: getApiOrganizationsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/members\n  method: get\n  operationId: getApiOrganizationsOrganization_idMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/invitations\n  method: get\n  operationId:\
  \ getApiOrganizationsOrganization_idInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/registration-fields\n  method: get\n  operationId: gETorganizationsorgdomainsregistrationFieldscredentialIdtldExtraFieldsextendedAttributesTheRegistrarTLDRequiresAtRegistrationEgusNexuspurposeeucaAgreementsGenericAcrossRegistrarsViaMethodExists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/transfer-preflight\n  method: get\n  operationId: gETorganizationsorgdomainstransferPreflightnametldTheHandfulOfReasonsAnInboundTransferUsuallyFailsCheckedBeforeSubmitInsteadOfDiscoveredFiveDaysLaterReadOnlyRegistrationDataTheDomainIsntInTheOrgYet\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domain-findings\n  method: get\n  operationId: gETdomainFindingsTheAdvisorAcrossTheOrganisation3935OnlyWhatCountsRankedMostUrgentFirstAndOneFindingPerCauseSoARefusedRegistrarKeyIsOneItemNamingItsDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/overview\n  method: get\n  operationId: gETdomainsoverviewTheDomainsOverviewTab3936SeeDomainOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/settings-plan\n  method: get\n  operationId: gETdomainssettingsPlanPerDomainWhoDoesWhatBeforeABulkSettingsChange3939AReadTheChangeItselfGoesThroughEachSettingsOwnEndpointWhichAuditsItPerDomain\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/email-protection-plan\n  method: get\n  operationId: gETdomainsemailProtectionPlanEmailProtectionForSeveralDomainsAtOnceFromTheOverview3946AReadLikeTheSettingsPlanEachDomainsPlanIsEmailProtectionsAndTheApplyIsTheZonesOwnEmailProtectionEndpointOncePerZoneSoEveryWriteIsPreviewedAndAuditedPerDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/caa-protection-plan\n  method: get\n  operationId: gETdomainscaaProtectionPlanCAAForSeveralDomainsAtOnceFromTheOverviewsCAALine3946AReadTheApplyIsEachZonesOwnCaaProtectionEndpointSoEveryWriteIsPreviewedCheckedAgainstItsCertificatesAndAuditedPerDomainRoutesAsemailProtectionPlan\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/track\n  method: post\n  operationId: pOSTdomainstrackAddATrackedDomainByName3940ItsRegistrationFactsComeFromTheRegistryNeverFromThisRequestTheOnlyInputIsTheName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/domains\n  method: get\n  operationId: getApiOrganizationsOrganization_idDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/{id}\n  method: get\n  operationId: getApiOrganizationsOrganization_idDomainsId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/{id}\n  method: put\n  operationId: putApiOrganizationsOrganization_idDomainsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/domains/{domain_id}/archive\n  method: post\n  operationId: archiveADomainKeepTheRowStopShowingItInTheList588\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /api/organizations/{organization_id}/domains/{domain_id}/unarchive\n  method: post\n  operationId: bringAnArchivedDomainBackIntoTheWorkingList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/domains/{domain_id}/contacts\n  method: get\n  operationId: getApiOrganizationsOrganization_idDomainsDomain_idContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/{domain_id}/contacts\n  method: post\n  operationId: postApiOrganizationsOrganization_idDomainsDomain_idContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/domains/{domain_id}/contacts/{contact_id}\n  method: delete\n  operationId: deleteApiOrganizationsOrganization_idDomainsDomain_idContactsContact_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/domains/{domain_id}/pricing\n  method: get\n  operationId: gETorganizationsorgdomainsdomainpricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/{domain_id}/actions\n\
  \  method: get\n  operationId: gETorganizationsorgdomainsdomainactionsFetchCurrentDomainActionFromTheProviderproviderSpecificEgTransIP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/{domain_id}/ns-health\n  method: get\n  operationId: gETorganizationsorgdomainsdomainnsHealthChecksEachNameserverTCPPort53Reachability+AuthoritativeDelegation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/{domain_id}/setup\n  method: get\n  operationId: gETdomainsdomainsetupHowTheDomainIsSetUpAndWhatRunsOnIt3937SeeDomainSetup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/{domain_id}/registry-record\n\
  \  method: get\n  operationId: gETdomainsdomainregistryRecordWhatTheRegistryItselfSays3937EPPStatusCodesCreatedAndUpdatedDatesAndTheRawRDAPOrWHOISAnswerAskedOnlyWhenSomeoneOpensTheDisclosureThroughThePlatformWideDeduplicatedLookupTheDropCatchChecksUseAndNeverForAnOrganisationWeMayNotReachOutFor1599ADemoFixturesNamesAreInvented\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/{domain_id}/advisor\n  method: get\n  operationId: gETdomainsdomainadvisorTheAdvisorAlone3935ForThePageToReReadAfterAChangeATogglesResponseCarriesTheDomainNotItsFindingsAndANameserverCheckStoresAResultThePageLoadedBefore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/{domain_id}/capabilities\n  method: get\n  operationId:\
  \ gETorganizationsorgdomainsdomaincapabilitiesWhichRegistrarActionsAreAvailableForThisDomainTheRegistrarImplementsTheMethodANDwhereTheProviderExposesPerTLDInfoEgTransIPTheTLDSupportsItDrivesTheUIGreyOutSoWeNeverShowAToggleThatWouldJust422\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/{domain_id}/whois\n  method: get\n  operationId: gETdomainsdomainwhoisTheRegistrysRawAnswerForTheDomainPagesWHOISView\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/domains/{domain_id}/history\n  method: get\n  operationId: getApiOrganizationsOrganization_idDomainsDomain_idHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /api/organizations/{organization_id}/domains/{domain_id}/epp-code\n  method: get\n  operationId: gETorganizationsorgdomainsdomaineppCodeFetchesTheEPPauthCodeLiveFromTheProviderneverStored\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/contacts\n  method: get\n  operationId: getApiOrganizationsOrganization_idContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/contacts\n  method: post\n  operationId: postApiOrganizationsOrganization_idContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/contacts/{id}\n  method: get\n  operationId: getApiOrganizationsOrganization_idContactsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/contacts/{id}\n  method: put\n  operationId: putApiOrganizationsOrganization_idContactsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/contacts/{id}\n  method: delete\n  operationId: deleteApiOrganizationsOrganization_idContactsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/dns/address-move\n  method: get\n  operationId: whatMovingWouldChangeTheRecordsOnTheServerorTheGivenOnesWithWhatEachBecomesTheOnesLeftOutAndWhyTheMonitorsThatFollowAndTheServersToChooseFromChangesNothing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/sync\n  method: post\n  operationId: postApiOrganizationsOrganization_idDnsZonesDnsZone_idSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/zone-file\n\
  \  method: get\n  operationId: downloadTheZoneAsABINDMasterFile638\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/history\n  method: get\n  operationId: gETorganizationsorgdnsZoneszonehistoryWhatHappenedToThisZone708Phase7\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/changes\n  method: get\n  operationId: theZonesRecordedChangesNewestFirstGroupedByTheOperationThatMadeThem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/restore-preview\n  method: get\n  operationId: whatRestoringTheZoneToJustAfterABatchWouldChangeChangesNothing\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-changes/undo\n  method: post\n  operationId: undoOneChangeOrAWholeBatchOfThem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/outside-changes\n  method: get\n  operationId: theZonesOutsideChangesNobodyHasDecidedOnNewestFirstEachWithWhatTheRecordWasAndIs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/leftovers\n  method: get\n  operationId:\
  \ theRecordsProposedForRemovalEachWithItsReasonAndTheEvidenceBehindIt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/live-mismatch\n  method: get\n  operationId: gETStoredBesideLivePerRecordWithTheCause\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/released-address\n  method: get\n  operationId: checkOneAddressAgainstTheOrganizationsReleasedAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/record-context\n  method: get\n  operationId: whatEveryRecordInTheZonePointsAtAndWhatUsesItKeyedByRecordId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/points-at\n  method: get\n  operationId: whatAValueWouldPointAtBeforeItIsSavedTheRecordDialogstheNewValueIs3958\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/dns-records/{record_id}/label\n  method: put\n  operationId: setOrClearWhatARecordIsFor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/server-addresses\n  method:\
  \ get\n  operationId: getApiOrganizationsOrganization_idDnsZonesDnsZone_idServerAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones\n  method: get\n  operationId: getApiOrganizationsOrganization_idDnsZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}\n  method: get\n  operationId: getApiOrganizationsOrganization_idDnsZonesDnsZone_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/dns-records\n  method: get\n  operationId: getApiOrganizationsOrganization_idDnsZonesDnsZone_idDnsRecords\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/dns-records\n  method: post\n  operationId: createARecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/dns-records/{record_id}\n  method: get\n  operationId: getApiOrganizationsOrganization_idDnsZonesDnsZone_idDnsRecordsRecord_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/dns-records/{record_id}\n  method: put\n  operationId: updateARecord\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/dns-zones/{dnsZone_id}/dns-records/{record_id}\n  method: delete\n  operationId: deleteARecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/provider-credentials\n  method: get\n  operationId: getApiOrganizationsOrganization_idProviderCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/organizations/{organization_id}/provider-credentials/health\n  method: get\n  operationId: lightweightHealthSummaryForTheNavBadgeHowManyEnabledIntegrationsAreCurrentlyDegradeddown24HFailureRateGETproviderCredentialshealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/provider-credentials/{providerCredential_id}\n  method: get\n  operationId: gETproviderCredentialASingleAccountForItsDetailPage483Phase3Counts+Health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-overview\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/organizations/{organization_id}/cloud-savings\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudSavings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/right-sizing\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idRightSizing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/quiet-hours\n  method: get\n  operationId: getApiOrganizationsOrganization_idQuietHours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/scheduled-actions\n  method: get\n  operationId: getApiOrganizationsOrganization_idScheduledActions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/server-operations/{serverOperation_id}\n  method: get\n  operationId: oneOperationAndItsStepsForTheProgressCardWhileItRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers\n  method: get\n  operationId: listServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}\n  method: put\n  operationId: putApiOrganizationsOrganization_idCloudServersCloudServer_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/untrack\n  method: post\n  operationId: stopTrackingThisServerLeaveItRunningAtTheProviderStopListingItHere600\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/address-references\n\
  \  method: get\n  operationId: whatElseInInfraNestStillNamesThisServersAddress1673\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/pricing\n  method: put\n  operationId: setAManualMonthlyPrice276P2FlagsThePriceAsManualSoProviderSyncStopsOverwritingIt\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/reset-pricing\n  method: post\n  operationId: resetAManualPriceBackToTheProvidersLastSyncednetPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/backup-pricing\n  method: put\n  operationId: overrideTheBackupsLine276StoredNETnullClearsItBackToTheProvidersPriceHetznersComputedRuleIndependentOfTheBasePriceSoOverridingBackupsNeverFlipsTheBaseToManual\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/metrics\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idMetrics\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/agent-sent\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idAgentSent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/workloads\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idWorkloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/workload-change\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idWorkloadChange\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/day\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/coming-up\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idComingUp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/events\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idEvents\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/unusual\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idUnusual\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/alert-rule-evidence\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idAlertRuleEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/reboots\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idReboots\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/ports\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idPorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/new-ports\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idNewPorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/role\n  method: get\n  operationId: getApiOrganizationsOrganization_idCloudServersCloudServer_idRole\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/reboot-plan\n  method: get\n  operationId: whatASafeRebootOfThisServerWouldDoWhichLoadBalancerItLeavesWhoCarriesTheTrafficMeanwhileAndAtAboutWhatCPUWhichFallbackAppliesAndWhichOtherServersAreWaitingForARebootTooWithTheProviderItGoesThroughTheMonitorsItWaitsForAndWhyItIsWaitingForTheDialogsWords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations/{organization_id}/cloud-servers/{cloudServer_id}/operations\n  method: get\n  operationId: theOperationsOnThisServerThatAreRunningOrFinishedInTheLastWeekNewestFirst\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (128\
  \ KB total) ---\n# Full source: https://artifacts.apis.io/infranest/agentic-access/infranest-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/infranest/agentic-access/infranest-agentic-access.yml
summary_line: 360 operations · 102 acting · 15 human-in-the-loop
tags:
- Company
- Infrastructure
- DNS
- Monitoring
- SSL
- Cloud
---
