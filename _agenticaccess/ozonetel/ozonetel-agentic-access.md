---
acting_count: 69
action_class_counts:
  acting: 69
  connected: 28
api_specs:
- filename: ozonetel-agent-api-openapi.yml
  format: yaml
  label: Ozonetel Agent API
  slug: ozonetel-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-agent-api-openapi.yml
- filename: ozonetel-aht-api-openapi.yml
  format: yaml
  label: Ozonetel AHT API
  slug: ozonetel-aht-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-aht-api-openapi.yml
- filename: ozonetel-campaign-api-openapi.yml
  format: yaml
  label: Ozonetel Campaign API
  slug: ozonetel-campaign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-campaign-api-openapi.yml
- filename: ozonetel-campaign-reports-api-openapi.yml
  format: yaml
  label: Ozonetel Campaign Reports API
  slug: ozonetel-campaign-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-campaign-reports-api-openapi.yml
- filename: ozonetel-chat-campaign-api-openapi.yml
  format: yaml
  label: Ozonetel Chat Campaign API
  slug: ozonetel-chat-campaign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-chat-campaign-api-openapi.yml
- filename: ozonetel-default-api-openapi.yml
  format: yaml
  label: Ozonetel Default API
  slug: ozonetel-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-default-api-openapi.yml
- filename: ozonetel-disposition-api-openapi.yml
  format: yaml
  label: Ozonetel Disposition API
  slug: ozonetel-disposition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-disposition-api-openapi.yml
- filename: ozonetel-reports-api-openapi.yml
  format: yaml
  label: Ozonetel Reports API
  slug: ozonetel-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-reports-api-openapi.yml
- filename: ozonetel-sms-api-openapi.yml
  format: yaml
  label: Ozonetel SMS API
  slug: ozonetel-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-sms-api-openapi.yml
consequence_counts:
  physical: 1
  read: 28
  safety-critical: 16
  write: 52
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 16
kind: agentic-access
layout: agentic-access
method: generated
name: Ozonetel Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /APIServices/campaignControl/chat
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /APIServices/campaignControl/chat
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /APIServices/campaignControl/chat
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /APIServices/campaignControl/chat
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /APIServices/campaignControl/chat
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /APIServices/campaignControl/chat
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /APIServices/campaignControl/inbound
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /APIServices/campaignControl/outbound
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /APIServices/campaignControl/outbound
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /APIServices/campaignControl/outbound
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ca_apis/AgentManualDial
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ca_apis/AgentManualDial
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ca_apis/CallControl_V4
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ca_apis/CallControl_V4
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ca_apis/PhoneManualDialSkillWise
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /ca_apis/PhoneManualDialSkillWise
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /OzonetelSMS/api.php?action=sendBulkSMS
operation_count: 97
overview: 'Ozonetel exposes 97 API operations that an AI agent could call, of which 69 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 52 write, 1 physical, and 16 safety-critical.


  16 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ozonetel
provider_slug: ozonetel
slug: ozonetel-agentic-access
source_filename: ozonetel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/ozonetel-add-campaign-bulk-data-v4-api-openapi.yml, openapi/ozonetel-add-campaign-data-basic-authentication-api-openapi.yml,\n  openapi/ozonetel-add-campaign-data-bulk-v4-api-openapi.yml, openapi/ozonetel-add-campaign-data-in-java-api-openapi.yml,\n  openapi/ozonetel-add-campaign-data-token-authentication-api-openapi.yml, openapi/ozonetel-agent-authentication-api-openapi.yml,\n  openapi/ozonetel-agent-details-java-basic-api-openapi.yml, openapi/ozonetel-agent-details-java-token-api-openapi.yml,\n  openapi/ozonetel-agent-manual-dial-java-basic-api-openapi.yml, openapi/ozonetel-agent-manual-dial-java-token-api-openapi.yml,\n  openapi/ozonetel-agent-manual-dial-skill-basic-java-api-openapi.yml, openapi/ozonetel-agent-manual-dial-skill-token-java-api-openapi.yml,\n  openapi/ozonetel-agent-state-summary-basic-auth-api-openapi.yml, openapi/ozonetel-agent-state-summary-token-auth-api-openapi.yml,\n  openapi/ozonetel-available-campaigns-basic-api-openapi.yml,\
  \ openapi/ozonetel-available-campaigns-token-api-openapi.yml,\n  openapi/ozonetel-average-handling-time-basic-authentication-api-openapi.yml, openapi/ozonetel-average-handling-time-token-authentication-api-openapi.yml,\n  openapi/ozonetel-call-control-in-conference-basic-java-api-openapi.yml, openapi/ozonetel-call-control-in-conference-java-token-api-openapi.yml,\n  openapi/ozonetel-call-recording-pause-unpause-api-openapi.yml, openapi/ozonetel-campaign-phone-number-lookup-basic-auth-api-openapi.yml,\n  openapi/ozonetel-campaign-phone-number-lookup-token-auth-api-openapi.yml, openapi/ozonetel-change-agent-state-java-basic-api-openapi.yml,\n  openapi/ozonetel-create-agent-java-basic-new-api-openapi.yml, openapi/ozonetel-create-agent-java-token-api-openapi.yml,\n  openapi/ozonetel-create-block-number-group-java-basic-api-openapi.yml, openapi/ozonetel-create-block-number-group-java-token-api-openapi.yml,\n  openapi/ozonetel-create-chat-campaign-api-openapi.yml, openapi/ozonetel-create-chat-campaign-api-token-auth-api-openapi.yml,\n\
  \  openapi/ozonetel-create-outbound-campaign-api-openapi.yml, openapi/ozonetel-create-phone-number-java-basic-api-openapi.yml,\n  openapi/ozonetel-create-phone-number-java-token-api-openapi.yml, openapi/ozonetel-delete-agent-java-api-openapi.yml,\n  openapi/ozonetel-delete-agent-java-token-api-openapi.yml, openapi/ozonetel-delete-block-number-grp-basic-api-openapi.yml,\n  openapi/ozonetel-delete-block-number-grp-java-api-openapi.yml, openapi/ozonetel-delete-campaign-data-java-basic-api-openapi.yml,\n  openapi/ozonetel-delete-campaign-data-java-token-api-openapi.yml, openapi/ozonetel-delete-chat-campaign-api-basic-auth-api-openapi.yml,\n  openapi/ozonetel-delete-chat-campaign-api-token-auth-api-openapi.yml, openapi/ozonetel-delete-phone-number-java-basic-api-openapi.yml,\n  openapi/ozonetel-delete-phone-number-java-token-api-openapi.yml, openapi/ozonetel-delete-schedule-campaign-data-java-basic-api-openapi.yml,\n  openapi/ozonetel-delete-schedule-campaign-data-java-token-api-openapi.yml,\
  \ openapi/ozonetel-deletebulkdata-api-openapi.yml,\n  openapi/ozonetel-deletebulkdata-basic-api-openapi.yml, openapi/ozonetel-dynamin-did-api-openapi.yml,\n  openapi/ozonetel-edit-agent-details-java-basic-api-openapi.yml, openapi/ozonetel-edit-agent-details-java-token-api-openapi.yml,\n  openapi/ozonetel-edit-phone-number-java-basic-api-openapi.yml, openapi/ozonetel-edit-phone-number-java-token-api-openapi.yml,\n  openapi/ozonetel-eventsubscriptionapi-api-openapi.yml, openapi/ozonetel-fetch-cdr-by-pagination-basic-1-api-openapi.yml,\n  openapi/ozonetel-fetch-cdr-by-pagination-token-1-api-openapi.yml, openapi/ozonetel-fetch-cdr-by-ucid-basic-1-api-openapi.yml,\n  openapi/ozonetel-fetch-cdr-by-ucid-token-1-api-openapi.yml, openapi/ozonetel-fetch-cdr-details-basic-1-api-openapi.yml,\n  openapi/ozonetel-fetch-cdr-details-token-1-api-openapi.yml, openapi/ozonetel-generate-token-for-reports-api-openapi.yml,\n  openapi/ozonetel-get-abandon-calls-basic-authentication-api-openapi.yml, openapi/ozonetel-get-abandon-calls-token-auth-api-openapi.yml,\n\
  \  openapi/ozonetel-get-block-number-group-java-basic-api-openapi.yml, openapi/ozonetel-get-block-number-group-java-token-api-openapi.yml,\n  openapi/ozonetel-get-campaign-status-basic-api-openapi.yml, openapi/ozonetel-get-campaign-status-token-api-openapi.yml,\n  openapi/ozonetel-get-customer-hold-data-cdr-basic-api-openapi.yml, openapi/ozonetel-get-customer-hold-data-cdr-token-api-openapi.yml,\n  openapi/ozonetel-get-disposition-list-dispositionv2-api-openapi.yml, openapi/ozonetel-get-disposition-list-dispositionv2-token-auth-api-openapi.yml,\n  openapi/ozonetel-get-phone-number-details-basic-api-openapi.yml, openapi/ozonetel-get-phone-number-details-token-api-openapi.yml,\n  openapi/ozonetel-get-wa-templates-api-openapi.yml, openapi/ozonetel-kreditbeecampaign-preprod-api-openapi.yml,\n  openapi/ozonetel-phone-manual-dial-java-basic-api-openapi.yml, openapi/ozonetel-phone-manual-dial-java-token-api-openapi.yml,\n  openapi/ozonetel-phone-manual-dial-skillwise-java-api-openapi.yml, openapi/ozonetel-phone-manual-dial-skillwise-token-api-openapi.yml,\n\
  \  openapi/ozonetel-release-agent-phone-number-basic-auth-api-openapi.yml, openapi/ozonetel-release-agent-phone-number-token-auth-api-openapi.yml,\n  openapi/ozonetel-schedule-campaign-data-basic-api-openapi.yml, openapi/ozonetel-schedule-campaign-data-java-token-api-openapi.yml,\n  openapi/ozonetel-set-campaign-status-basic-1-api-openapi.yml, openapi/ozonetel-set-campaign-status-token-1-api-openapi.yml,\n  openapi/ozonetel-set-disposition-dispositionv2-api-openapi.yml, openapi/ozonetel-set-disposition-dispositionv2-token-auth-api-openapi.yml,\n  openapi/ozonetel-sms-bulk-api-openapi.yml, openapi/ozonetel-update-block-number-group-java-basic-api-openapi.yml,\n  openapi/ozonetel-update-block-number-group-java-token-api-openapi.yml, openapi/ozonetel-update-chat-campaign-api-basic-auth-api-openapi.yml,\n  openapi/ozonetel-update-chat-campaign-api-token-auth-api-openapi.yml, openapi/ozonetel-update-outbound-campaign-api-openapi.yml,\n  openapi/ozonetel-whatsappbulkapis-api-openapi.yml\ndescription:\
  \ Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 97\n  by_action_class:\n    acting: 69\n    connected: 28\n  by_consequence:\n    write: 52\n    safety-critical: 16\n    read: 28\n    physical: 1\n  human_in_the_loop_required: 16\noperations:\n- path: /cloudAgentRestAPI/index.php/AddCampaignBulkDataV4/addBulkData/format/json\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/AddCampaignData\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AddCampaignDataBulkV4\n  method: post\n  operationId: addCampaignDataBulkV4\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/CAToken/generateToken\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/AddCampaignData\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CAServices/AgentAuthenticationV2/index.php\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/AgentDetails\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/AgentDetails\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/AgentManualDial\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/AgentManualDial\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/AgentManualDial\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ca_apis/AgentManualDial\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ca_reports/summaryReport\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_reports/summaryReport\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/getAvailableCampaigns\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/getAvailableCampaigns\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/aht\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/aht\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/CallControl_V4\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ca_apis/CallControl_V4\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /CAServices/Call/Record.php\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/campaigns/lookup/phoneNumber\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/campaigns/lookup/phoneNumber\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/changeAgentState\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/createAgent\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/createAgent\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /ca_apis/createBlockNumber\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/createBlockNumber\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /APIServices/campaignControl/chat\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n   \
  \ escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /APIServices/campaignControl/chat\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /APIServices/campaignControl/outbound\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ca_apis/PhoneManageV2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/PhoneManageV2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/deleteAgent\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/deleteAgent\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/deleteBlockNumber\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/deleteBlockNumber\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/deleteCampaignData\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/deleteCampaignData\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /APIServices/campaignControl/chat\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /APIServices/campaignControl/chat\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ca_apis/PhoneManageV2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/PhoneManageV2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/deleteScheduledData\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/deleteScheduledData\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/DeleteBulkData\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/DeleteBulkData\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /APIServices/dynamic/did/update\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/updateAgent\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/updateAgent\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/PhoneManageV2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/PhoneManageV2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/subscribe\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/subscriptions/list\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/un-subscribe\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_reports/fetchCdrByPagination\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_reports/fetchCdrByPagination\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /ca_reports/fetchCdrByUCID\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_reports/fetchCdrByUCID\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_reports/fetchCDRDetails\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_reports/fetchCDRDetails\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_reports/CAToken/generateToken\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/abandonCalls\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/abandonCalls\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/getBlockNumber\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/getBlockNumber\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/campaignStatus\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/campaignStatus\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_reports/getCustomerHoldData\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_reports/getCustomerHoldData\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/DispositionAPIV2\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/DispositionAPIV2\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/PhoneManageV2\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca_apis/PhoneManageV2\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chat/OzonetelMetaAPI/message_templates/waba_id/{waba_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /APIServices/campaignControl/inbound\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /APIServices/campaignControl/outbound\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ca_apis/PhoneManualDial\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/PhoneManualDial\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/PhoneManualDialSkillWise\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ca_apis/PhoneManualDialSkillWise\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /ca_apis/ReleaseFwpNumber\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/ReleaseFwpNumber\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/CampaignScheduledData\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/CampaignScheduledData\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/setCampaignStatus\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/setCampaignStatus\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/DispositionAPIV2\n  method: post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/DispositionAPIV2\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /OzonetelSMS/api.php?action=sendBulkSMS\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /ca_apis/updateBlockNumber\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca_apis/updateBlockNumber\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (33 KB total) ---\n# Full source: https://artifacts.apis.io/ozonetel/agentic-access/ozonetel-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/ozonetel/agentic-access/ozonetel-agentic-access.yml
summary_line: 97 operations · 69 acting · 16 human-in-the-loop
tags:
- Company
- CX Platform
- Cloud Communications
- Contact Center
---
