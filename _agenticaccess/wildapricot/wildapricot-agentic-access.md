---
acting_count: 57
action_class_counts:
  acting: 57
  connected: 48
api_specs:
- filename: wildapricot-admin-api-openapi.yml
  format: yaml
  label: WildApricot Admin API
  slug: wildapricot-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wildapricot/refs/heads/main/openapi/wildapricot-admin-api-openapi.yml
consequence_counts:
  physical: 24
  read: 48
  write: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wildapricot Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/contactfields
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountId}/contactfields/{contactFieldId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountId}/invoices/{invoiceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /accounts/{accountId}/invoices/{invoiceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/payments/{donationId}/AllocateRefundToDonation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/payments/{donationId}/UnallocateFromDonation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountId}/payments/{paymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /accounts/{accountId}/payments/{paymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/payments/{paymentId}/AllocateInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/payments/{paymentId}/AllocateRefundToPayment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/payments/{paymentId}/UnallocateFromPayment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/{accountId}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountId}/refunds/{refundId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /accounts/{accountId}/refunds/{refundId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounts/{accountId}/store/orders/{orderNumber}/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/{accountId}/ApprovePendingMembership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/{accountId}/GenerateInvoiceForEventRegistration
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/{accountId}/GenerateInvoiceForPendingMembership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/{accountId}/RejectPendingMembership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/{accountId}/VoidInvoice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/{accountId}/email/SendEmail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/{accountId}/email/SendEmailDraft
operation_count: 105
overview: 'WildApricot exposes 105 API operations that an AI agent could call, of which 57 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 48 read, 33 write, and 24 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WildApricot
provider_slug: wildapricot
slug: wildapricot-agentic-access
source_filename: wildapricot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wildapricot-admin-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 105\n  by_action_class:\n    connected: 48\n    acting: 57\n  by_consequence:\n    read: 48\n    write: 33\n    physical: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: GetApiResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  operationId: GetAccountsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: GetAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/contacts\n  method: get\n  operationId: GetContactsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/contacts\n  method: post\n  operationId: CreateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/contacts/me\n  method: get\n  operationId: GetCurrentContactInfo\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/contacts/{contactId}\n  method: get\n  operationId: GetContactDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/contacts/{contactId}\n  method: put\n  operationId: UpdateContactDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/contacts/{contactId}\n  method: delete\n  operationId: DeleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/{accountId}/AcceptTermsOfUse\n  method: post\n  operationId: AcceptTermsOfUse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/contactfields\n  method: get\n  operationId: GetContactFieldDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/contactfields\n  method: post\n  operationId: CreateContactFieldDefinition\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/contactfields/{contactFieldId}\n  method: put\n  operationId: UpdateContactFieldDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/contactfields/{contactFieldId}\n  method: delete\n  operationId: DeleteContactFieldDefinition\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/savedsearches\n  method: get\n  operationId: GetSavedSearchesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/savedsearches/{savedSearchId}\n  method: get\n  operationId: GetSavedSearchDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/pictures/{pictureId}\n  method: get\n  operationId: GetPictureContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/pictures\n  method: post\n  operationId: UploadPicture\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/attachments/{attachmentId}\n  method: get\n  operationId: GetAttachmentContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/attachments/GetInfos\n  method: get\n  operationId: GetAttachmentInfos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /accounts/{accountId}/attachments/Upload\n  method: post\n  operationId: UploadAttachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/membershiplevels\n  method: get\n  operationId: GetMembershipLevelsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/membershiplevels/{levelId}\n  method: get\n  operationId: GetMembershipLevelDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/bundles\n\
  \  method: get\n  operationId: GetMembershipBundlesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/bundles/{bundleId}\n  method: get\n  operationId: GetMembershipBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/membergroups\n  method: get\n  operationId: GetMembershipGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/membergroups/{memberGroupId}\n  method: get\n  operationId: GetMembershipGroupDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /rpc/{accountId}/ApprovePendingMembership\n  method: post\n  operationId: ApprovePendingMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/{accountId}/RejectPendingMembership\n  method: post\n  operationId: RejectPendingMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/events\n\
  \  method: get\n  operationId: GetEventsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/events\n  method: post\n  operationId: CreateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/events/{eventId}\n  method: get\n  operationId: GetEventDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/events/{eventId}\n  method: put\n  operationId: UpdateEvent\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/events/{eventId}\n  method: delete\n  operationId: DeleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/{accountId}/CloneEvent\n  method: post\n  operationId: CloneEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /accounts/{accountId}/EventRegistrationTypes\n  method: get\n  operationId: getEventRegistrationTypesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/EventRegistrationTypes\n  method: post\n  operationId: CreateEventRegistrationType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/EventRegistrationTypes/{typeId}\n  method: get\n  operationId: GetEventRegistrationTypeDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /accounts/{accountId}/EventRegistrationTypes/{typeId}\n  method: put\n  operationId: UpdateEventRegistrationType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/EventRegistrationTypes/{typeId}\n  method: delete\n  operationId: DeleteEventRegistrationType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/eventregistrations\n  method: get\n  operationId: GetEventRegistrationsList\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/eventregistrations\n  method: post\n  operationId: CreateEventRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/eventregistrations/{event_registration_id}\n  method: get\n  operationId: GetEventRegistrationDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/eventregistrations/{event_registration_id}\n  method: delete\n  operationId: DeleteEventRegistration\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/eventregistrations/{event_registration_id}\n  method: put\n  operationId: UpdateEventRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/{accountId}/CheckInEventAttendee\n  method: post\n  operationId: CheckInEventAttendee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/{accountId}/RegisterFromWaitlist\n  method: post\n  operationId: RegisterFromWaitlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/invoices\n  method: get\n  operationId: GetInvoicesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/invoices\n  method: post\n  operationId: CreateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n   \
  \ token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/invoices/{invoiceId}\n  method: get\n  operationId: GetInvoiceDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/invoices/{invoiceId}\n  method: put\n  operationId: UpdateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/invoices/{invoiceId}\n  method: delete\n\
  \  operationId: DeleteInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/{accountId}/GenerateInvoiceForPendingMembership\n  method: post\n  operationId: GenerateInvoiceForPendingMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/{accountId}/GenerateInvoiceForEventRegistration\n  method: post\n  operationId: GenerateInvoiceForEventRegistration\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/{accountId}/VoidInvoice\n  method: post\n  operationId: VoidInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/payments\n  method: get\n  operationId: GetPaymentsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/payments\n  method: post\n  operationId: CreatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/payments/{paymentId}\n  method: get\n  operationId: GetPaymentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/payments/{paymentId}\n  method: put\n  operationId: UpdatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/payments/{paymentId}\n  method: delete\n  operationId: DeletePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/payments/{paymentId}/AllocateInvoice\n  method: post\n  operationId: AllocateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/payments/{paymentId}/AllocateRefundToPayment\n  method: post\n  operationId: AllocateRefundToPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/payments/{donationId}/AllocateRefundToDonation\n  method: post\n  operationId: AllocateRefundToDonation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/payments/{paymentId}/UnallocateFromPayment\n  method: post\n  operationId: UnallocateFinanceDocumentFromPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/payments/{donationId}/UnallocateFromDonation\n  method: post\n  operationId: UnallocateFinanceDocumentFromDonation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/paymentAllocations\n  method: get\n  operationId: GetPaymentAllocationsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/refunds\n  method: get\n  operationId: GetRefundsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/refunds\n  method: post\n  operationId: CreateRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/refunds/{refundId}\n  method: get\n  operationId: GetRefundDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/refunds/{refundId}\n  method: put\n  operationId: UpdateRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/refunds/{refundId}\n  method: delete\n  operationId: DeleteRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n\
  \    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/tenders\n  method: get\n  operationId: GetTendersList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/tenders\n  method: post\n  operationId: CreateTender\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/tenders/{tenderId}\n  method: get\n  operationId: GetTenderDetails\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/tenders/{tenderId}\n  method: put\n  operationId: UpdateTender\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/tenders/{tenderId}\n  method: delete\n  operationId: DeleteTender\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/auditLogItems\n  method: get\n\
  \  operationId: GetAuditLogItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/auditLogItems/{itemId}\n  method: get\n  operationId: GetAuditLogItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/donationfields\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/donationfields\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/donationfields/{donationFieldId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/donationfields/{donationFieldId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/donations\n  method: get\n  operationId: GetDonationsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/donations/{donationId}\n  method: get\n  operationId: GetDonationDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/donations/{donationId}\n  method: put\n  operationId: UpdateDonation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/SentEmails\n  method: get\n  operationId: GetSentEmailsLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /accounts/{accountId}/SentEmails/{emailId}\n  method: get\n  operationId: GetSentEmailDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/EmailDrafts\n  method: get\n  operationId: GetEmailDraftsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/EmailDrafts/{draftId}\n  method: get\n  operationId: GetEmailDraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/EmailDrafts/{draftId}\n  method: delete\n  operationId: DeleteEmailDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/SentEmailRecipients\n  method: get\n  operationId: SentEmailRecipientList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - auto\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rpc/{accountId}/email/SetEmailDraftSchedule\n  method: post\n  operationId: SetEmailDraftSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/{accountId}/email/GetEmailDraftPreview\n  method: post\n  operationId: GetEmailDraftPreview\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/{accountId}/email/SendEmailDraft\n  method: post\n  operationId: SendEmailDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/{accountId}/email/SendEmail\n  method: post\n  operationId: SendEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - auto\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\n\n# --- truncated at 32 KB (35 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/wildapricot/refs/heads/main/agentic-access/wildapricot-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wildapricot/refs/heads/main/agentic-access/wildapricot-agentic-access.yml
summary_line: 105 operations · 57 acting
tags:
- Membership Management
- Associations
- Nonprofit
- Events
- Payments
---
